= (\__/)   __________________________   (\__/)
= (=^~^)/) Welcome to EpicKitty's BNC (\(^~^=)
= (")(")   ‾‾\BNC Log Grabber Bot/‾‾‾   (")(")
            ‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾

Requirements:


	 - This bot must be able to grab a user's logs depending on their username and network

	 - Not much authentication is required as this bot will run on partyline, therefor the user
	   must already be authenticated with my bouncer to get into the partline. This will also
	   allow for the user variable to be grabbed when looking at the file paths.

	 - Using the bot, the users should be able to either download their logs (Via DCC or temp 
	   web link) or view them. Entire logs can be viewed fairly fast since partyline doesn't 
	   have throttling.

	 - The bot must then be compatable with all znc versions, maybe have config items for things
	   such as log location, bnc details, web server location and output link

	 - Like my other bots, this might be built on the Phergie framework just to make things simple
	   and so that all of my bots can have exchangable plugins.


Commands:

	ViewLog - Outputs a log file from the user's logs (ViewLog <network> <log>)

	GetLog - Generates a download link for a log file (GetLog <network> <log>)

	ListNetworks - Lists all of the networks that the user has logs for (ListNetworks)

	ListLogs - Lists all of the log files for that network (ListLogs <network>)

	GetAll - Generates a download link for all of the logs (GetAll <network>)


Config Items:

	server - the znc server you want to connect to (Default: ipv4.epickitty.uk)

	port - the port that the server will run on (Default: 1234)

	ssl - Is the connection using SSL (Default: false)

	username - The bot's username (Default: Log)

	password - The bot's password (Default: password)

	zncdir - The location of znc (Default: /home/znc/.znc/)

	downloadmode - What type of download do you want DCC/WEB (Default: WEB)

	webroot - Location to put the log files for the user to download (Default: /var/www/epickitty.uk/public_html/private/)

	outputroot - Web link that should be generated when files are stored in the webroot (Default: https://epickitty.uk/private/)

	owner - The username for the owner of the bot. For admin commands (Default: ?EpicKitty)

Description:

	This bot will work as a secure znc log grabber. It will contain different methods of outputting the logs to the users.
	This bot will not have any strict security measures as it should soly be used as a partyline bot. Opening it to irc network
	would be un-needed and pointless as it would require a lot more code written to allow the bot to work out who is who and also
	most irc networks have blocked DCC transfers since they can be used illegaly. Once this bot is fully working and functioning,
	the source code will be released here on this github repo but for now, this will be all.

	The sole purpose for this will be to allow users to download their own logs without admins having to manually get the logs for
	the users to download. Like most bots, this will be taking the stress out of sharing the logs to your bouncer users.

	Who knows, this could actually be successful since it doesn't require a webpage or extra security messures before it can work.
	The only things this requires is ZNC and the Log module running.
