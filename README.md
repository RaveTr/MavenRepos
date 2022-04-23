# Dimensional Swords Maven

This is the maven branch for a joke mod of mine, initially intended to be a private mod between a friend and I.

## Importing mods into your workspace

In order to import Dimensional Swords into your workspace, you must add the following to your **build.gradle** file:

### Repository

```
	maven {
		name = "DimensionalSwordsMaven" 
		url = "https://raw.github.com/RaveTr/MavenRepos/Dimensional-Swords-Forge"
	}
```

### Dependency

```
implementation fg.deobf("com.slepderp:DimensionalSwords:1.16.5-1.0") //You could probably get by adding *${project.dimensionalswords}* after the mod name
```

### IMPORTANT: Do NOT add any of these inside the dependencies or repositories in the buildscript of your *build.gradle* file!

Good luck in whatever mod you're making.
