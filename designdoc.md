# RLBots design doc


#### Can explain why you think this is better than other options?
I think that individual downloads are better then botpacks because of the following reasons
* the user ends up opnly with the bots he wants to have
* system can be extended by prodiding different repos for different usecases, for example an special repo containing bots that attended to an certain event
* updating and packaging bots can be shifted to the bot maker

#### What the drawbacks of this?
repos needs to be maintained

#### Also I'm confused at how it actually works on a meta level.
the program will read repo files in json format form the saved repos, it defenes info for the hub page lile the repo link, the gamemodes the developer supports, etc. on cloning the github only the bot folder (contains packaging.json) will be downloaded to the bot folder and can be deleted with the hub if the user doesnt want it anymore.

#### How is this implemenred in the GUI?
new page alongside main.html what does execute the hub features.

#### How do we track the usage?
not ;) verry privacy friendly

#### How do we make sure that only safe bots get passed on to users?
Just as now we can't garuanty safetyness when we will increase the amount of bots in the botpack. on that point there is only improvement to make to do this automaticly. i can try to implement the following with help of others

* after download of the bot source, the code can be scanned for imports of libaries that are not needed for the development of the bot but have the propabillity to be misused. for example packages that use os interfaces or networks or the file system
* Maintain an stableTrusted repo with tested bots where those bots are hosted on the rlbots github

#### How are bots updated
we will require the bots to have an packaging.json in the main folder of their bot, containing the bot info and other info (local botinfo so unlisted bots in development can be filtered locally with the listed bot if the user wants) what can be compared to the repo info (or i read packaging.json in that repo, not really sure yet). if the version is different the user can choose to update the bot.

#### How do we make sure bots are working?
we can't, just as now. as the game and rlbots are evolving compactabillity can not be guaranteed. We can probide stable bots in our stableTrusted repo and maintain it right by updating and testing, if needed dropping bots from stableTrusted when they aren't updated anymore and are not working correctly
