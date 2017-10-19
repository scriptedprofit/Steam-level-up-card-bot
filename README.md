# Steam-level-up-card-bot
A bot which buys and sell steam trading card sets. It will check which sets the user has.

Features Commands:
!buy [Amount in keys] Buy an amount of sets.

!sell [Amount in keys] Sell an amount of cards to the bot

!level [Level] Check how much it will cost and how many sets it takes to get to a certain level.This is calculated from your current level.

!check Check how many sets that you have not crafted yet are buyable, how much that will cost and how many sets the bot has in total.

!sellcheck Check how many sets you own, that you can sell to the bot.

!help Extra help

Demo: http://steamcommunity.com/profiles/76561198257636063/

.
.
.
.
SET-UP:

How to get your shared_secret & identity_secret:

1: Go to the SDA(Steam Desktop Authenticator) directory. If you have encryption disabled go to step 3.

2: Open SDA and hit "Manage Encryption". Fill in your encryption key and when asked to create a new one leave the text box blank. This 
will disable encryption.

3: Head over to the maFiles folder and open the file named after your accounts SteamID64.

4: Search the file for shared_secret:"XXXXXXXXXXXXXX=", instead of XXX it should have a code there, it always ends with =

5: Do the same for identity_secret, it will look similar.


How to set up a server with DigitalOcean
1: Add funds, and create a Droplet. Hit "One Click Apps" and select NodeJS.

2: Once created, download Putty and Filezilla: https://filezilla-project.org/ & 
http://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html

3: Open Putty, fill in the IP address sent to your e-mail and wait for the command prompt to open. Once opened fill in username "root" and the password sent to your email. You can copy your password in your email and paste it in Putty using right click, you wont see your password!

4: It will ask you to fill in the password again, fill it in and fill in a new password and confirm it.

5: Once you're done run the command: npm install -g forever. This allows the server to run the bot without a Putty window being opened.

6: Now open FileZilla and connect to your server, username = root and the password is the password you've just set, port = 22.

7: Drag the bot files in, wait for this to complete and head back to Putty.

8: Run the command: npm i

9: To start your bot run this command in Putty: forever start index.js
g

Then your bot should be running!

Make sure to fill in the config!
