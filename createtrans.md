### Introduction

In the case where you don't find your native langage on the list of avaible one, there is an easy way to create your own one. The only requirement is a little bit of patient.
Roll up your slaves and let's begin !

### Structure

In order to add a new translation, you have in reality 2 files to translate. The first one in the web app and second one is the lua part. You will be able to find these directories at the following path :
 * Lua :`/gamma/lang/`
 * Web : `/translations/`
 
### Create files

* Web : You will have to create on the translation directory a file which will respect the following syntax : lang_COUNTRY.json . Here is an example : en_EN.json for english langage in England or en_US.json for english in the USA.
* Lua : You will have to create on the translation directory a file which will respect the following syntax : lang.lua . Here is an example : en.lua for english langage or fr for french. You don't have to specify any country.

> For this tutorial, i'm going to create an language called Baguette (what's wrong ? No one told you about Baguette's country ?), so i'm going to create bg_BG.json and bg.lua (abbreviation for baguette) files. 

The first file bg_BG.json go to `/translations/` and the second one bg.lua go to `/gamma/lang/`. Now, let's open theses files and put our hands dirty.

### Web translation

After oftening your translation file, you will have to follow the json syntax but also put all needed words. I would like to remind you that there is no reason for concern, all will be explain.
The easy way to create a new translation is to copy the content of en_EN.json. Paste it into your new translation file and take a look to lines.
You should see this (approximately) :
```json
#Infos related to this translation
infos:
    name: 'English'
    author: 'Arnaud'
# If you find any mistake, feel free to report this issue on : https://github.com/ArnaudDevelopper/GammaLang
global:
    see: 'See'
    name: 'Name'
    version: 'Version'
    validate: 'Validate'
    add: 'Add'
    cancel: 'Cancel'
    edit: 'Edit'
    next: 'Next'
    previous: 'Previous'
    submit: 'Submit'
    send: 'Send'
    error: 'Error'
    success: 'Success'
    warning: 'Warning'
    state: 'State'
    author: 'Author'
    created: 'Created at'
    updated: 'Updated at'
    update: 'Update'
    type: 'Type'
    search: 'Search'
    by: 'By'
    yes: 'Yes'
    no: 'No'
    details: 'Details'
    lastresponse: 'Last response'
    actions: 'Actions'
    image: 'Image'
    order: 'Order'
    date: 'Date'
    new: 'New'
    active: 'Active'
    expiration: 'Expiration date'
    options: 'Options'
    title: 'Title'
    content: 'Content'
    steamid: 'STEAM ID'
    setdefault: 'Set as default'
Etc...
```
On the top of the file, change name by the complete name of your language and author by your name. For my new language, it will be :
```json
#Infos related to this translation
infos:
    name: 'Baguette'
    author: 'Arnaud'
```
Now, let's begin the hardest part : translate each line :expressionless:. **You only have to translate the string contained in ''. If you don't, the translation will not work.**
After each line translated, web part is finished, you can save your file. Let's move to lua part !

### Lua translation

Like before, start by opening your translation file. Copy the content of en.lua and paste it to your file. You would find something lile this :
```lua
--[[----------------------------------------------------------
    Gamma - A freaking donation system made in France
    Languages.French <-> French baguette translation for Gamma
    @author Gabriel Santamaria <gaby.santamaria@outlook.fr>
    Copyright 2020 Gabriel Santamaria
    LICENSE : See LICENSE.txt
    Licensed to : {{ user_id }}
------------------------------------------------------------]]
local en = {

}

return en
```
Change `en` on local and return by your language abrevation. For mine, it would be `local bg` and `return bg`. In the same way as before, you will have to translate each line.
After all finished, save your file.

### Change your current language

* For web, go to your admin panel in general settings and select your language.
* For lua, go to `/gamma/lang/config.lua` and look for **Gamma.Lang.Locale** variable. Then, change the string associated to this variable with your language's abreviation.

When finished, restart your server.It's finished, you created your own language !

### Publish your language for all users

If the traduction you created is your native langage, feel free to publish it for all users. How ?
Go to our github page(https://github.com/ArnaudDevelopper/GammaLang) and create a push create with your file.

> You can have Gamma for free if you are native to the langage you're publishing ! Just add to your lua or web translation your mail adress and you will win Gamma for free. 