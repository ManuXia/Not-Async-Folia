<div align=center>
    <img src="./not-async-folia.png">
    <br /><br />
    <p>Fork of <a href="https://github.com/PaperMC/Folia">Folia</a> working towards a strictly single-threaded world execution model</p>
</div>

## 🦴 Overview

- Fork of Folia working towards a strictly single-threaded world execution model(not fully achieved, but we will try)

## ✨ Features

- ✅ Removes multithreading completely
- ✅ Great for benchmarking single-threaded server performance
- ✅ Useful for analysing Folia’s overhead vs traditional single-threaded execution
- ✅ Illegal thread access is no longer prevented, detected, or reported. 
- ✅ TPS spikes
- ✅ More lag due to watchdog, ticking regions
- ✅ Slower chunk generation
- ✅ Cross region latency

It's noe multithreaded, but is still in tick regions(or else it's not going to be 
folia, but paper), ticks all regions, keeps folia watchdog, all region on the 
same thread.Plugins using RegionScheduler.run() / EntityScheduler.run() will be 
strictly on the same thread. 

## ⏬ Installing

- All stable release are in our Release page

## 🔥 Building

./gradlew applyAllPatches
./gradlew createMojmapPaperclipJar

## FAQ

### What server types can benefit from Not-Async-Folia?


### What hardware will Folia run best on?


## Plugin compatibility

There should be one and only one thread (we are still working on it),
async catchers are removed, bukkit plugins should run fine? Expect
to see tps spikes, random issues, item dupe, entity disappearing/teleporting,
region deadlock, random crashes, ghost entities/items/blocks

So, have your expectations for compatibility at ?.

## Get Support & Bug reporting

If you enounter any issue or bug, please tell us by opening an issue
**Please Remember to:**
- Provide full logs and relating enviornment(Version, Plugins etc.)
- Reproduction steps if possible.

## 💼 To Do

- Scheduler system to become strictly single-threaded
- Chunk load/gen to become strictly single-threaded
- Eneity AI, behavior and pathfinding to become strictly single-threaded
- Force synchronous IO.

## 🤝 Contributing
We greatly appreciate your contribution to this project.

Please open an issue with your well done work, thanks!

## 🎉 Contributers

@

@

@

@

We are very grateful for their contributions to this project; without them, Not-Async-Folia would not be possible.

## ⭐ Please Give a Star

Every free ⭐ motivates us to continue working on this project.


**!? What's the Point ?!**
