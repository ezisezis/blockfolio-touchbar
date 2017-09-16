# Blockfolio for your touch bar
A simple script that retrieves your blockfolio balance and displays it in touch bar. When icon is pressed, it displays the portfolio value in BTC. Then switches back to default.

![touchbar screenshot](https://github.com/ezisezis/blockfolio-touchbar/blob/master/touchbar.png)
## Installation
### Things you will need
 - Macbook Pro with a touch bar
 - node JS to run the script
 - Better Touch Tool to display the icons. It has a 45-day trial period and later pay-as-much-as-you-want scheme.
 - A mobile phone who has Blockfolio application installed on it

 ### Setup steps
1. Install node version manager as explained here: https://github.com/creationix/nvm#installation
2. Do ```nvm install 8.4.0``` which will install version 8.4.0 of NodeJS on your Macbook. This is needed to execute the script that retrieves the information from Blockfolio API.
3. Clone the repository inside ```Documents``` directory on your Mac. Open terminal and execute these commands:
 - ```cd Documents```
 - ```git clone git@github.com:ezisezis/blockfolio-touchbar.git```
 - ```cd blockfolio-touchbar```
 - ```npm install```
 - ```chmod +x wrapper.sh```
4.  Open configuration.js in any text editor and change the deviceID to the one found in Blockfolio. You can see that in the app by opening it and navigating to upper right corner (the three vertical dots) and at the bottom. You can also "Copy your device ID".
5.  Download and install Better Touch Tool from here: https://www.boastr.net/downloads/ 
6. Once installed, open preferences from the menu bar icon. and go to Touch bar -> Manage Presets -> Import -> Select the blockfolio.json file that is part of this repo and now you should see the items in touch bar. It automatically adds to icons - one for dollar and one for euro pair, remove the one you don't need. If you cloned the repository in another location, then you will have to change paths in JSON file ```BTTTouchBarAppleScriptString``` attribute before importing them. 
7. Optionally add extra presets to display the value of other crypto currencies - https://github.com/krunkosaurus/bettertouchtool-crypto
