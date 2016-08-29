Author
-----
Hussein Bakri

Title of the script
--------------------
CreateXUserAccountsForOpenSim

script description 
------------------
This Linux bash shell script create x number of user accounts (for Non-Player Characters NPC) in OpenSim server and save the user accounts details to a CSV file called OpenSimUsers.csv.
This CSV file can be fetched as it is to my tool  libOMVMobilityModels hosted here: https://github.com/HusseinBakri/libOMVMobilityModels

libOMVMobilityModels is an NPCs QoS stress and mobility tool that uses LibOpenMetaverse which can be found here   https://github.com/openmetaversefoundation/libopenmetaverse)

libOMVMobilityModels allows you to choose from 6 mobility models for your NPCs:
[1] StayingStillWithoutYawFor3minutes , [2] StayingStillWithYawFor3minutes , [3] RandomWalkFor3minutes ///[4] RandomRunFor3minutes , [5] RandomFlyFor3minutes , [6] RandomTeleportFor3minutes ///Enjoy!

In a nutshell you can now create hundreds of user accounts automatically using this shell script and load the resulting  CSV file to my libOMVMobilityModels tool which can allow your avatars to act upon one of the mobility models specified. 

License
-------
GNU GLP v3 License - you are free to distribute, change, enhance and include any of the code of this shell script in your tools. I only expect  adequate attribution of this work. The attribution should include the title of the script, the author and the site or document where the script is taken from.

Logic of the script
------------------
This script uses the GNU Screen command ( https://www.gnu.org/software/screen/) to script OpenSim console commands. I will write later on my website (husseinbakri.org) a detailed guide of how this is done due to the scarcity of information on the technique especially when it comes to scripting OpenSim console commands and getting information back from OpenSim console.

It  should be noted that you can script OpenSim server console commands through any web programming language (like PHP) through the help of the RemoteAdmin Module kindly see this: http://opensimulator.org/wiki/RemoteAdmin. 

In this case you can use http://opensimulator.org/wiki/RemoteAdmin:admin_create_user. 
Nevertheless this shell script do the job. This script can be improved in many ways (it is not perfect and never meant to be). I am happy to hear comments! Enjoy!

Usage
-----
1) Drop the bash shell script into the bin folder of your OpenSim server

2) change its permissions if required: chmod +x createXUsersAccountsOpenSim

3) While in bin directory run it as follows: ./createXUsersAccountsOpenSim

Warning:
-------
Don't use this Linux bash shell script as it is. Please change the  code to suit your world especially when giving enough time for your OpenSim world to load and enough time to shutdown. I might update the script later (if time allows) to take arguments. Enjoy!
