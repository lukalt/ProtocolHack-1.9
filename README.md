#PaperSpigot Protocol Hack 1.7

This is my fork of the PaperSpigot Project which aims to support all Minecraft Versions from 1.7.2 to 1.9. Installation instructions can be found below. This 

PaperSpigot 1.7 itself is no longer maintained by the original developers.


###Quick Installation Guide:
####Windows:
Make sure you installed git and maven.

Open the Git Bash and clone this repo by typing `git clone https://github.com/lukas81298/protocolhack-1.9.git`

Type `cd ProtocolHack-1.9`

Init the submodules `git submodule update --init`

Apply the patches: `./applyPatches.sh`

Recompile the sources: `mvn clean install`

The final .jar file can be found in `/PaperSpigot-Server/target`

How To
-----------

Init the submodules : `git submodule update --init`

Apply Patches : `./applyPatches.sh`

### Create patch for server ###

`cd PaperSpigot-Server`

Add your file for commit : `git add <file>`

Commit : `git commit -m <msg>`

`cd ..`

Create Patch `./rebuildPatches.sh`

### Create patch for API ###

`cd Paperspigot-API`

Add your file for commit : `git add <file>`

Commit : `git commit -m <msg>`

`cd ..`

Create Patch `./rebuildPatches.sh`




Compilation
-----------

We use maven to handle our dependencies.

* Install [Maven 3](http://maven.apache.org/download.html)
* Clone this repo and: `mvn clean install`
