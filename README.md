# SlepDerp's Maven Repository

This repository contains branches, which have mavens for all the minecraft mods that I've developed thus far.

## Importing mods into your workspace

In order to import mods, you must add the following to your **build.gradle** file:

###Repository

```
	maven {
		name = "ModMaven" //Just name it *Mod Name*Maven or something, or something you can identify it with
		url = "https://raw.github.com/RaveTr/MavenRepos/*Insert branch name here*" //Branch name should obviously be the exact same as it is on the repository's page
	}
```

###Dependency

```
implementation fg.deobf("com.slepderp:ModName:MinecraftVersion-ModVersion") //You could probably get by adding *${project.modid}* after the mod name
```

###IMPORTANT: Do NOT add any of these inside the dependencies or repositories in the buildscript of your *build.gradle* file!

If any of my mods have external dependencies, just add them via the method mentioned above, or follow their steps (if they have anything extra you might need to add). 

Good luck in whatever mod you're developing.
