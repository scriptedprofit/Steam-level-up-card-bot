# Steam-level-up-card-bot
[b]Features Commands[/b]
!buy [Amount in keys] Buy an amount of sets.
!sell [Amount in keys] Sell an amount of cards to the bot
!level [Level] Check how much it will cost and how many sets it takes to get to a certain level. This is calculated from your current level.
!check Check how many sets that you have not crafted yet are buyable, how much that will cost and how many sets the bot has in total.
!sellcheck Check how many sets you own, that you can sell to the bot.
!help Extra help
Commands for admins !block [steamid64] When a user spams and is removed by the bot all admins will receive a message containing their steamid64. They can use !block to make the bot block them, preventing them from adding the bot again.
Configuration
Everything you should set is in the config file
A group to which the bot invites people when they add the bot/accept a trade from the bot.
Which game the bot should play. You can set as many as you'd like to idle hours. You can also set it to play a non steam game, to list your prices for instance.
A comment that the bot will post on a user's profile after trading.
The max hours the bot will have users on his friends list. Users will be notified and removed after this amount of hours. This only takes effect if the user has not used the bot in the set amount of hours.
A maximum amount of messages per second (Spam filter). If a user spams they will be removed and admins will be notified.
Buy rate.
Sell rate.
The maximum amount of sets the buy will buy at a time. (For example maximum of 50 of the same set at a time)
People that are able to sell. This is handy for private sellers.
You are able to set custom messages.
Limitations. You are able to set a cap on the amount of keys you'd want the bot to send per trade. You are also able to set the highest level that can be used while using !level. This will prevent people from creating infinite loops and thus crashing the bot.
Which keys are accepted. This does not necessary have to be keys. You can set which item is used as currency and from what game.
Thats all about it. Feel free to add me https://steamcommunity.com/id/schokodidek89/
DEMO
Demo: http://steamcommunity.com/profiles/76561198257636063/

SET-UP:
How to get your shared_secret & identity_secret:
1: Go to the SDA(Steam Desktop Authenticator) directory. If you have encryption disabled go to step 3.
2: Open SDA and hit "Manage Encryption". Fill in your encryption key and when asked to create a new one leave the text box blank. This will disable encryption.
3: Head over to the maFiles folder and open the file named after your accounts SteamID64.
4: Search the file for shared_secret:"XXXXXXXXXXXXXX=", instead of XXX it should have a code there, it always ends with =
5: Do the same for identity_secret, it will look similar.

How to set up a server with DigitalOcean
1: Add funds, and create a Droplet. Hit "One Click Apps" and select NodeJS.
2: Once created, download Putty and Filezilla: https://filezilla-project.org/ & http://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html
3: Open Putty, fill in the IP address sent to your e-mail and wait for the command prompt to open. Once opened fill in username "root" and the password sent to your email. You can copy your password in your email and paste it in Putty using right click, you wont see your password!
4: It will ask you to fill in the password again, fill it in and fill in a new password and confirm it.
5: Once you're done run the command: npm install -g forever. This allows the server to run the bot without a Putty window being opened.
6: Now open FileZilla and connect to your server, username = root and the password is the password you've just set, port = 22.
7: Drag the bot files in, wait for this to complete and head back to Putty.
8: Run the command: npm i
9: To start your bot run this command in Putty: forever start index.js

Then your bot should be running!

Make sure to fill in the config!
