# Overview

This mod is a compatibility patch between my two major compilation mods [Subtle Polish: A Collection of Fixes and Enhancements](https://steamcommunity.com/sharedfiles/filedetails/?id=2522974089) and [Silfae's Portraits: Revisited](https://steamcommunity.com/sharedfiles/filedetails/?id=2596417938).  Both of them make changes to the same Pop jobs files, and thus need a patch so that all the changes are applied concurrently.

# Changes

Overwrites two game files, which are also overwritten in each of the source mods, in order to make their changes work together:

* `common/pop_jobs/03_worker_jobs.txt`
* `common/pop_jobs/06_event_jobs.txt`

## Compatibility

Only use this mod if you are using [Subtle Polish: A Collection of Fixes and Enhancements](https://steamcommunity.com/sharedfiles/filedetails/?id=2522974089) and/or [Silfae's Portraits: Revisited](https://steamcommunity.com/sharedfiles/filedetails/?id=2596417938).  Because the only conflicts are between the packed mods ["Agrarian" Idyll for Lithoids](https://steamcommunity.com/sharedfiles/filedetails/?id=2510669821) and [Animated Holosphere Portraits: Revisited](https://steamcommunity.com/sharedfiles/filedetails/?id=2592592503), this mod can be used a a compatibility patch between both collection mods, one of the collection mods and the conflicting single mod, or between just the two conflicting single mods.

Built for Stellaris version 3.1.2 "Lem."  Not compatible with achievements.

## Changelog

* 1.0.0 Initial version

## Source Code

Hosted on [GitHub](https://github.com/corsairmarks/combined_compatibility)

### Development Notes

It is best to clone this repository into `<Stellaris User's Directory>/Paradox Interactive/Stellaris/mod`, and then make a connection to the `mod` folder via a `*.mod` file's `path` property.  That will ensure the game can see the files, and also that CWTools will parse them.  Also note that the README.md file exists in the `mod` directory but is symbolically linked in the root directory.