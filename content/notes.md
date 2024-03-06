+++
title = "Notes"
template = "notes.html"
+++

Notes about the upkeep of the CreeperCraft server
## Connecting
- Website: [Link](https://creepercraft.online)
- IP: `creepercraft.online`
- Port: `19132`
- Tutorial blog: [Link](https://shockbyte.com/billing/knowledgebase/66/How-to-Join-a-Minecraft-PocketorBedrock-Edition-Server.html)
- Tutorial video: [Link](https://www.youtube.com/watch?v=wA_Wknnw3qc)
- You need to be whitelisted
## Plugins
We do any plugins because bedrock doesn't support them. There are a few different ways to do them but none of them are good enough so might as well keep it all vanilla. There is [GeyserMC](https://geysermc.org/) for packet translation but it doesn't work on most consoles without [BedrockConnect](https://github.com/Pugmatt/BedrockConnect) and people would have to configure their Xbox which is too tricky. Therefore, no plugins 😔
## Sustainability
The server should be up for at least 3 years, ideally at least 5 years. World backups should *always* have an offsite backup (see [S3 Glacier](https://aws.amazon.com/s3/storage-classes/glacier/)) and ideally an onsite backup on another disk. In the future the server should be migrated from DigitalOcean and into a mini-pc. The server should aim for 5 players with 0 issues, 10 players at max without really any lag.
## Checklist
- [ ] Get a server to get it up and running; probably DigitalOcean
- [ ] Download the Bedrock server package (see [here](https://www.minecraft.net/en-us/download/server/bedrock))
- [ ] Connect DNS up to `creepercraft.online` in [NameCheap](https://www.namecheap.com/)
- [ ] Get the [whitelist](https://www.google.com/search?client=firefox-b-d&q=bedrock+how+to+configure+whitelist) configured
	- [ ] Get peoples names
	- [ ] Add to the whitelist
	- [ ] Test/restart the server
- [ ] Change the website to say about the new stuff in [Plugins](#plugins)