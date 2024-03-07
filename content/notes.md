+++
title = "Notes"
template = "notes.html"
+++
Notes about the upkeep of the CreeperCraft server
## Connecting
- Website: [Link](https://creepercraft.online)
- IP: `join.creepercraft.online`
- Java edition:
	- Port: `25565` (default)
	- Tutorial video: [Link](https://www.youtube.com/watch?v=RlLsdP-F3lM)
- Bedrock edition:
	- Port: `19132` (default)
	- Tutorial video: [Link](https://www.youtube.com/watch?v=wA_Wknnw3qc)
	- Workaround: [Link](https://github.com/Pugmatt/BedrockConnect?tab=readme-ov-file#tutorials)
- You need to be whitelisted
## Plugins
### History
Originally, the server was intended to be completely vanilla on Bedrock, but it has been migrated to a Java server. The server runs on Java to enable plugins and PC player to be able to properly play as Java is generally nicer to work with than the more locked-down Bedrock edition. Here was the original thinking:

> We do any plugins because bedrock doesn't support them. There are a few different ways to do them but none of them are good enough so might as well keep it all vanilla. There is GeyserMC for packet translation but it doesn't work on most consoles without BedrockConnect and people would have to configure their Xbox which is too tricky. Therefore, no plugins 😔

Now that the server is running [GeyserMC](https://geysermc.org/) and a lot of players wont even need [BedrockConnect](https://github.com/Pugmatt/BedrockConnect), players on both the Java and Bedrock editions can play nicely, with Java plugins being [compatible](https://wiki.geysermc.org/geyser/faq/#what-plugins-dont-work-with-geyser) enough. Any plugins that are added to the server should be *light* and not really affect the vanilla experience too much.
### Current
Below is a list of the plugins which are currently installed:
- [GeyserMC](https://geysermc.org/) – Allows Bedrock players to connect and play
- [Chunky](https://hangar.papermc.io/pop4959/Chunky) – Preloads chunks for better performance
### Possible
Below is a list of plugins that might be fun to add to the server:
- Rare head drops on kills (1 in 1000 chance?)
- Minor economy mod so we can trade; like item shop signs?
- Maybe some kind of pipeline thing so we can make factories
## Sustainability
The server should be up for at least 3-4 years, ideally at least 5 years. World backups should *always* have an offsite backup (see [S3 Glacier](https://aws.amazon.com/s3/storage-classes/glacier/)) and ideally an onsite backup on another disk. In the future the server should be migrated from DigitalOcean and into a mini-pc. The server should aim for 5 players with 0 issues, 10 players at max without really any lag.
## Upkeep
### Checklist
Next steps/chores for the server to be completed:
- [x] Get a server to get it up and running; probably DigitalOcean
- [x] Download the Bedrock server package (see [here](https://www.minecraft.net/en-us/download/server/bedrock))
- [x] Connect DNS up to `creepercraft.online` in [NameCheap](https://www.namecheap.com/)
- [ ] Get the [whitelist](https://www.google.com/search?client=firefox-b-d&q=bedrock+how+to+configure+whitelist) configured
	- [ ] Get peoples names
	- [ ] Add to the whitelist
	- [ ] Test/restart the server
- [x] Change the website to say about the new stuff in [Plugins](#plugins)
- [x] Migrate the server to use the Java edition
	- [x] Figure out the best base for it post-Spigot
	- [x] Download the files required for it
	- [x] Install GeyserMC
	- [x] Make a new startup script to properly use the resources
	- [x] Set the seed to `CreeperCraft` like the previous one
	- [x] Ensure it all works on PC and Xbox again
- [ ] Figure out how to do backups
- [ ] Style all the website up a bit more :)
