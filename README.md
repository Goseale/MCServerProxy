# DFProxy

[![Travis CI](https://img.shields.io/travis/DFProxy/DFProxy)](https://travis-ci.org/DFProxy/DFProxy)
[![Minecraft](https://img.shields.io/badge/minecraft-1.13.2-informational)](https://minecraft.gamepedia.com/Java_Edition_1.13.2/)
[![js-semistandard-style](https://img.shields.io/badge/code%20style-semistandard-brightgreen.svg?style=flat)](https://github.com/standard/semistandard)

***__DISCLAIMER:__*** **This is NOT an official DiamondFire project.  It is NOT managed by DiamondFire and DiamondFire is NOT responsible for the contents or use of this project.**

**The managers of this project are LittleWhole, SiebeDW, and Goseale.**

DFProxy is a proxy that tunnels your connection to DiamondFire - a central proxy with many users that enables many unprecendented features. Client-side mods like [DFTools](https://github.com/KSashaDF/DFTools) (previously DFUtils) were only able to achieve what was limited by the client - but DFProxy is a new take on modifying and enhancing the [DiamondFire experience](https://www.mcdiamondfire.com).

Things like custom commands, custom actions (send resource pack, send to plot) and more server-based features are all included in DFProxy.
## Developers
SiebeDW, Goseale, LittleWhole - and you, the contributor!
## Installation
### Prerequisites
In order to run DFProxy, you need at least Node v10.0 or later.

Also, you will need to put your credentials in a configuration file stored on your local machine that *nobody* can access.
#### Why do I need to put my credentials?
DFProxy works by creating a server on localhost and creating a client with your player on that server. Because of the way Minecraft servers work, Mojang needs to authenticate your user with valid credentials. You need to specify your credentials in a configuration file so DFProxy can authenticate it with Mojang.

We, the developers, do not store your credentials. No one that does not have access to your computer can access it. Your credentials are stored on your PC **only**. It is entirely safe to type in your credentials.

If we haven't gained your full trust, you can look at the code in this repository, or you can research a little about how Minecraft servers work technically.

**Never download DFProxy from forks, other repositories, or external sites. The only place where you should download DFProxy is in the DFProxy/DFProxy repo. You should only download from our [releases page](https://github.com/DFProxy/DFProxy/releases) and download the latest version only. Not adhereing to this warning may compromise the security of your Minecraft account.**
### Linux/macOS
1. Download the source code tarball from the releases page.
2. Unzip the tarball.
3. Open Terminal.
4. `cd` to the unzipped directory:
```sh
$ cd ~/DFProxy-v1.0.0
```
5. Edit `config.json` and enter your email and password that you want to log in with.
6. `cd` to the `src` folder:
```sh
$ cd ./src
```
7. Run index.js:
```sh
$ node index.js
```
8. Connect to `localhost:25566` and you're set!
## Usage
To use DFProxy, follow the installation procedure above. Once you connect to `localhost:25566` you should be in DiamondFire, tunneled by DFProxy. To make sure your connection is actually tunneled, upon joining you should see a title saying `[DFProxy] Your connection is tunneled!`

In order to use custom actions, place a SendMessage and send `DFPROXY|<ACTIONNAME>|<ARGS>`.

Run the /dfproxy command for a full list of all commands.
## Feature List
* More Commands
* Custom Actions (Send Resource Pack, Send To Plot, etc.)