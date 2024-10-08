# THIS IS A FORK!!!

This is a fork of the main repository.
The main purpose of this is to build the client at a certain point.

## Automated Nightly Builds

Every day it checks whether there are new commits to the upstream. If there are, it tries to
rebase this repo to the upstream, then starts a build.

## Manual Build

A "release" build is triggered when a tag is created. However (atm) there is no way to create only
a tag on GitHub w/o creating a release.
Hence steps below creates a release with a tag and deletes it.

1. Go to release https://github.com/kurorinchan/yet-another-anime-game-launcher/releases
2. "Draft a new release"
3. Create a tag name that follows X.Y.Z, all numbers. Preferrably something like 9999.Y.Z where Y and Z match those of the main repository. 9999 is a number where the main repo should never reach.
4. Give it any name (don't spend much time here, you will delete it later).
5. Wait for it to build until "Release X.Y.Z" is generated by the action. Download the artifacts you need.

Following steps are optional.

6. Delete the release (used only to create a tag) created in steps 3&4.
7. Publish the release (w/ the artifacts) created in step 5.

# Yet another anime game launcher (Yaagl)

## Current Supported Game Version: 
### GI: 5.0.0 OS/CN **
### HSR: 2.5.0 OS/CN
### ZZZ: 1.2.0 OS/CN

#### **: For Apple Silicon users: Sonoma 14.4 is required

## For Linux users
[Anime Games Launcher](https://github.com/an-anime-team/anime-games-launcher) is a universal linux launcher for anime games

<!-- ## Policy

Please don't link to this repository. If you really want to share it with people, just tell the project name __Yaagl__ and where to find (Github!) but __don't share/disclose the link__ unless it's a private message.

Do __not__ provide any forms of tutorial for _how to use Yaagl_ on public channels. (If you really want to do that, ask the project owner for permission first.)

Do __not__ mention the real name of the game or the game company, in code commits, issues, pr or dicussions. Use _The Anime Game_ or _The Anime Company_ instead.

Just follow these, or share and ruin this project for all other macOS (including Linux as well) players. -->

<!-- ### Hall of Shame

This is a list of people/organization violating Yaagl policies -->

## Is it safe?

Use it at your own risk. Or enjoying it with a new f2p account.

## Support

[Our Discord server](https://discord.gg/HrV52MgSC2) is the **ONLY** place providing support if you have any issue just using this application. 

**DON'T FILE AN ISSUE** unless it's a technical problem coming with a clear root cause. 

> Simply put _My game doesn't launch_ or _I can't login_ without telling any technical detail is not acceptable, please go to the Discord server instead of abusing Github Issues

**DON'T ASK FOR SUPPORT IN OTHER COMMUNITY**, especially the official one.

## Install

- Go to [Release](https://github.com/3Shain/yet-another-anime-game-launcher/releases/latest) and download the latest version.

- Uncompress and copy the resulting application to your `/Applications` folder. (Do not open the application from Downloads folder).

- Also make sure your game files aren't stored inside `/Applications`, use something inside your home folder instead, e.g `Games/GI`.
<!-- 
## Development (Outdated)

### Setup
```sh
git clone https://github.com/3Shain/yet-another-anime-game-launcher
cd yet-another-anime-game-launcher
pnpm install
./configure.sh
pnpm exec neu update
```


### Run
```sh
# CN
pnpm start
# Oversea
pnpm run start-hk4eos
```

### Build
```sh
node ./build-app.js
``` -->

## Uninstall (completely)
1. Drag app to the bin
2. Delete folder `~/Library/Application Support/Yaagl` or `~/Library/Application Support/Yaagl OS` if you are using oversea version. (For HSR and ZZZ the name of folder is slightly different)

## Related projects

* Custom `neutralinojs` binary from [3Shain/neutralinojs](https://github.com/3Shain/neutralinojs)
* [DXVK-macOS](https://github.com/Gcenx/DXVK-macOS)
* [MoltenVK](https://github.com/KhronosGroup/MoltenVK)

## Special thanks
* An Anime Team
* Krock, the game running on macOS can not come true without his patch (you can find the link to his work in this repository, while you have to make a little effort ;) )

* mkrsym1, tackled IMO the most challenging AC component. It's a really remarkable and mind-blowing achievement.
