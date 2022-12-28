**_DEPRECATED:_** As of the 3.4 "Cepheus" versions of Stellaris, there are no conflicts between "Subtle Polish: A Collection of Fixes and Enhancements" and "Silfae's Portraits: Revisited." Do not use this mod.

# Overview

This mod is a compatibility patch between my two major compilation mods [Subtle Polish: A Collection of Fixes and Enhancements](https://steamcommunity.com/sharedfiles/filedetails/?id=2522974089) and [Silfae's Portraits: Revisited](https://steamcommunity.com/sharedfiles/filedetails/?id=2596417938).  Both of them make changes to the same Pop jobs files, and thus need a patch so that their changes are applied concurrently.

As of Stellaris version 3.3 "Libra," this mod has drastically shrunk in size.  The only remaining conflicts are 4 miner-related jobs.

# Changes

Overwrites four jobs, which are also overwritten in each of the source mods, in order to make their changes work together:

* `miner`
* `scrap_miner`
* `cave_cleaner`
* `turtle_miner`

## Compatibility

Only use this mod if you are using [Subtle Polish: A Collection of Fixes and Enhancements](https://steamcommunity.com/sharedfiles/filedetails/?id=2522974089) and/or [Silfae's Portraits: Revisited](https://steamcommunity.com/sharedfiles/filedetails/?id=2596417938).  Because the only conflicts are between the packed mods ["Agrarian" Idyll for Lithoids](https://steamcommunity.com/sharedfiles/filedetails/?id=2510669821) and [Animated Holosphere Portraits: Revisited](https://steamcommunity.com/sharedfiles/filedetails/?id=2592592503), this mod can be used a a compatibility patch between both collection mods, one of the collection mods and the conflicting single mod, or between just the two conflicting single mods.

Built for Stellaris version 3.3 "Herbert."  Not compatible with achievements.

## Known Issues

Overriding a job causes the game to log errors. Expect to see four lines in the error.log file similar to these:

```
[00:00:21][game_singleobjectdatabase.h:147]: Object with key: miner already exists, using the one at  file: common/pop_jobs/23_combined_compatibility_worker_jobs.txt line: 7
[00:00:21][game_singleobjectdatabase.h:147]: Object with key: scrap_miner already exists, using the one at  file: common/pop_jobs/23_combined_compatibility_worker_jobs.txt line: 203
[00:00:21][game_singleobjectdatabase.h:147]: Object with key: cave_cleaner already exists, using the one at  file: common/pop_jobs/26_combined_compatibilit_event_jobs.txt line: 4
[00:00:21][game_singleobjectdatabase.h:147]: Object with key: turtle_miner already exists, using the one at  file: common/pop_jobs/26_combined_compatibilit_event_jobs.txt line: 125
```

## Changelog

* 1.0.0 Initial version
* 2.0.0 Update for compatibility with Stellaris version 3.2.2 "Herbert"
* 2.0.1 Do not gate the Angler job behind being an Anglers empire - some mods may add the ability to gain access to the job for non-Anglers
* 3.0.0 Update for compatibility with Stellaris version 3.3 "Libra"
    * Jobs are no longer full-file overwrites!
    * Only the relevant `miner`, `scrap_miner`, `cave_cleaner`, and `turtle_miner` jobs are overridden
    * Integrate additional changes from 3.3 to overridden content
* 3.0.1 Mark as deprecated - unnecessary in Stellaris 3.4 "Cepheus" and higher

## Source Code

Hosted on [GitHub](https://github.com/corsairmarks/combined_compatibility)

### Development Notes

It is best to clone this repository into `<Stellaris User's Directory>/Paradox Interactive/Stellaris/mod`, and then make a connection to the `mod` folder via a `*.mod` file's `path` property.  That will ensure the game can see the files, and also that CWTools will parse them.  Also note that the README.md file exists in the `mod` directory but is symbolically linked in the root directory.