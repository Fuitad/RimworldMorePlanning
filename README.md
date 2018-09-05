# MorePlanning

More Planning is a RimWorld mod that creates a new option in the "Architect" menu, called "Planning", with more options for planning.
                                     
Features:
- 10 customizable planning designations;
- Show/hide planning designations;
- Control planning opacity;
- Cut/copy/paste planning designations;
- An option for control if planning designations should be removed when something is built or deconstructed on top of it.
- Holding shift you can override others planning designations.

[More Planning - RimWorld Forum Topic](https://ludeon.com/forums/index.php?topic=31045.0)

[More Planning - Steam Workshop](http://steamcommunity.com/sharedfiles/filedetails/?id=881100382)

![Alt Text](http://i66.tinypic.com/244uzx4.png)

## Features
- Blue, red, green and yellow planning designations;
- Show/hide planning designations;
- Control planning opacity;
- Cut/copy/paste planning designations;
- An option for control if planning designations should be removed when something is built or deconstructed on top of it.
- Holding shift you can override others planning designations.

**This mod uses HugsLib (need to be installed and loaded before More Planning) and Harmony (comes with the mod, no need to be installed)**

## Contributors
- 53N4 - Spanish translation
- Dango998 - Chinese Simplified translation

## Building

### Stantard way

- Copy Assembly-CSharp.dll and UnityEngine.dll from RimWorldWin_Data/Managed/ folder to Source/MorePlanning/Library/
- Copy HugsLib.dll and 0Harmony.dll to Source/MorePlanning/Library

Compile the C# project Source/MorePlanning.

If you want to generate only the release files, use the semi-automated build or take a look at Gruntfile.js

### Semi-automated (Windows)

This method uses grunt to automate the build process. To setup:

- Install HugsLib
- Install node v8+
- Clone this repository inside mod folders. The name of the folder should not be MorePlanning.
- Run `npm install`
  - This will install required libs to execute build process.
- Run `node node_modules/grunt/bin/grunt setup`
  - This will copy dlls for modding from game folder

Finally, use `node node_modules/grunt/bin/grunt build` to build the mod.

`node node_modules/grunt/bin/grunt build-dist` can be used to create a folder called MorePlanning just with files needed to be released.