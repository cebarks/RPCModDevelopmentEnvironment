# RPCModDevelopmentEnvironment
A gradle project to allow developers to quickly get setup to develop mods for Retro Pixel Castles

This setup was tested using indev 12 unstable 2

currently the project supports the use of Intellij IDEA, but should also work with Eclipse.
If someone gets it working create a step by step and add it to this readme

## Setup Instructions (Intellij IDEA)
After cloning the repository open the *gradle.properties* file and change the *installDirectory* 
to point to your install of Retro Pixel Castles for example:
```
installDirectory=C:/Program Files (x86)/Steam/SteamApps/common/Retro-Pixel Castles
```

Once changed, open your command shell and run:

```
gradlew setupProject
```

Open the project with Intellij IDEA by double clicking build.gradle while in the open dialog box.

On the Import Project from Gradle dialog box:
```
1. check Create directories for empty content roots automatically
2. select .ipr(file based) for Project format
3. click OK
```

If asked to Open Existing Project select ***Delete Existing Project and Import***

The project should now be setup and ready to mod the game.
To test that everything is working:
```
1. On the right edge of the Intellij IDEA window there will be a gradle tab open it
2. In the popped out window expand RPC_Mod_Dev under All tasks
3. Double click the run task in the list that appears the game should begin to run
```
