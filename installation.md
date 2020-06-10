### Foreword

Gamma have some dependecies to work properly, make sure to have these installed into your hosting company. The list of these depedencies are documented into the welcome page of the installation process.
However, if you prefer a video tutorial, take a look to our youtube channel.

### Step 1 - Key verification

After purchasing the addon, you will receive a key which allow you to begin the installation of Gamma. After going to your website, you will have a field where you will have to paste your key.

### Step 2 - Database installation

Gamma needs a database to store few informations. On your hosting company, create a database. After creating this database, you should be able to access to these informations : 
* Database name
* Username
* Password
* Host adress

Fill all of these informations into the form and click on ``submit`` button. If the panel returns any error, please verify your informations or contact the support.

### Step 3 - General settings

Step 3 index all of general settings of your website. Please correctly fill all of these field even if you will be able to make any modification in the future.

### Step 4 - Administrator account

Administrator is your personnal account, he will be able to access to the admin panel. Make sure to have a strong password to prevent any unwanted intrusion by a third party.

### Set up addon

Go to your ``addon`` folder of your server and slip in the addon file of lua. Then, go to `gamma/config.lua` file and make your modifications. After this, launch your server and check in the console if this server happen : <br>

```bash
      * ***                                                              
    *  ****  *      A freaking donation system                           
   *  *  ****       made in France by Arnaud and Gabyfle                 
  *  **   **        © Copyright Arnaud and Gabyfle, All rights reserved  
 *  ***             Buy it at: https://gmodstore.com                     
**   **             ****    *** **** ****    *** **** ****       ****    
**   **   ***      * ***  *  *** **** ***  *  *** **** ***  *   * ***  * 
**   **  ****  *  *   ****    **  **** ****    **  **** ****   *   ****  
**   ** *  ****  **    **     **   **   **     **   **   **   **    **   
**   ***    **   **    **     **   **   **     **   **   **   **    **   
 **  **     *    **    **     **   **   **     **   **   **   **    **   
  ** *      *    **    **     **   **   **     **   **   **   **    **   
   ***     *     **    **     **   **   **     **   **   **   **    **   
    *******       ***** **    ***  ***  ***    ***  ***  ***   ***** **  
      ***          ***   **    ***  ***  ***    ***  ***  ***   ***   ** 
```
If it doesn't, please verify you don't make any mistake on `config.lua`. If not, please contact the support.