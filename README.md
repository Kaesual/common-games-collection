## The Common Games Collection

This repository is part of a broader effort to unify the build and setup process of amazing open source games for the web. I realized there are a lot of such games out there that have a somewhat working web version, but the build process is often cumbersome, not beginner friendly, and also requires a specific system setup to work.

I am collecting such games and make a basic set of changes:

1.) Provide a proper dockerized build system, so anyone can easily build the game. This way, the community can focus on game modifications, and there's one "centralized" place where build and setup can be discussed

2.) Provide a production-ready docker container for the game. This allows easy hosting for anyone.

3.) Provide a proper hosting setup. The game should be hostable behind a reverse nginx proxy (for easy https), and also on a freely choosable url / path.

4.) Enhanced UI/UX and browser integration. I add a simple, react-based loader frontend and sometimes additional game-specific components for easy integration and comfortable gameplay.

With those pre-requisites, I hope to build a growing collection of permissively licensed games and an ecosystem of gamers and contributors. There are decades of games made with love by artists, coders and - sometimes ancient - communities. I consider the Common Games Collection an effort to find the gold nuggets and artifacts that the internet gives us, and bring them together in one happy, easy to use collection.

## Games

**Luanti**

<img src="assets/luanti.png">

[Luanti](https://www.luanti.org/) is a fully Open Source voxel game engine that allows creation of games that look and feel like Minecraft, started in 2010 and written in c++. Until today, it has an active community of maintainers, contributors and players. There's also the [Luanti ContentDB](https://content.luanti.org/) where many games and mods can be found.

https://github.com/Kaesual/minetest-wasm

Updates:

- Added dockerized build environment and simple build command
- Builds a ready-to-use docker image (including all game assets)
- Added indexedDb world save synchronization and Zip Download + Restore
- Added custom overlay menu to configure synchronization and manage several other settings
- Added simple join code sharing for easy p2p play right in the browser
- Added customizable React based loader with many settings and options
- Added more pre-packed games for pre-selection in the loader
- Added configuration for playing in iframes (tricky header setup magic)

Next tasks:

- Use FileSystemDirectoryHandle (not iframe compatible though) to synchronize save games and game assets with a local folder instead of indexedDb (is probably required for running "bigger" game servers with friends, as indexedDb is more limited)

**Sauerbraten**

<img src="assets/sour.png">

[Sauerbraten](http://sauerbraten.org/) is a fully Open Source first person shooter that reminds of Quake 2 and early Unreal Tournament versions, started in 2004 and written in c++. It supports many game modes (ffa, insta, ctf...) and comes with **Game Server and Game Client built in**. Host it and play with others instantly.

https://github.com/Kaesual/sour

Updates:

- Added dockerized build environment and simple build
- Builds a ready-to-use docker image (including all game assets)
- Fixed a bug that would prevent keyboard events from being picked up in iframes

Next tasks:

- Fix some desync issues which can lead to undamageable or invisible players sometimes
- Enhance the assets build step to include more maps
- Build custom UI components for game and server management
- Long term: Tournaments and mma-based Matchmaking

## Vision

    "The old archives are full of sunken treasures, yearning to shine once more."

I want to build a growing Open Source Gaming community that is connected across projects. I intend to focus on Browser Gaming, and only on games that are licensed permissively and do not require any proprietary assets. Building and hosting should work simple and reliable across operating systems, and in a similar manner across projects so it's easy to get into other games. This ensures that the games are open for anyone to play and modify, and easy to discover and integrate.

As a long term goal, if these efforts are successful, I can imagine to create a decentralized game studio that can start with porting more Open Source Games to the browser, and might even create own games that are fully open at a later point.

I've been a gamer for more than 30 years, it was more fun in the early days to be honest. Many games feel soulless today, which feels even more true for Browsergames. And early access titles that will never fix their bugs have become so common that I think we really need a new model. I've learned that the most important task in doing something revolutionary is bringing together the right people first - so come join the collective if you feel aligned with this!

## Get in touch

The *Quest* of Common Games is to gather great Open Source games and make them available as browser versions. My goal is to bring together a community of players and developers, and bring "good old LAN party vibes" into the browser. Open Source game communities manage to unite people with different backgrounds and experiences, and are a place of collaboration and knowledge exchange. The goal of *browserifying* such games, *simplifying the tool chain* and *improving UI/UX* aims to make those games more accessible to a broader audience, and will make it easier to get involved.

There are several options to get in touch:

**Common Ground**

I'm the founder of a community platform named Common Ground, which runs on [app.cg](https://app.cg). It has many features similar to Discord or Slack, but it completely (and only) runs in the Browser. Custom software (like games) can be embedded into communities as iframes, and can be connected to the platform through an API.

That's my personal reason to build the Common Games Collection - all of the games are available as community plugins on app.cg. We're also planning to make the whole Common Ground platform available under a permissive community license this year - stay tuned! You can learn more about the project here: [Common Ground DAO on github](https://github.com/Common-Ground-DAO).

To play the game and get in touch for gaming, sign up and join the [Common Games Community](https://app.cg/c/commongames/). For the Common Ground project itself, join our [Common Ground Community](https://app.cg/c/commonground/).

**Discord**

I understand that not everyone is willing to sign up to a new platform, and that's fine. I am also running a Discord community for everyone else, so come join the [Common Games Community on Discord](https://discord.gg/FcK7PsdXtF) in case this is your preferred option.

**Reddit**

I also post updates about the game versions I make on reddit every once in a while. Still trying to find my flow here, but I'm normally posting game specific updates into the game subreddit, and also run my own [r/CommonGames](https://www.reddit.com/r/CommonGames/) subreddit where I post or crosspost. It's still new, but will probably become a good log of development efforts at some point.