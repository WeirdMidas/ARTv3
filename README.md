# ARTv3

## Basic, Efficient and Open-Source for enthusiasts
A very basic ART/JIT optimization, made for fun and also test the way ART/JIT is managed in Android and perhaps create formulas that work better in a real environment and in human perception.

---

> [RECOMMENDATION!]
> The module was made to run on 64-bit devices, older devices will not be compatible with it, only with 64-bit (that is, the most modern ones).

---

## Features
- Set SystemUi and System_Server to more efficient profiles for use. This improves the accuracy of memory management and even cleans it up with HeapTaskDaemon, the System_Server garbage collector. Apply speed-profile also for image compilation, and in turn, for ROM OAT updates.
- Apply at the end of each month (30 days after the module was installed), DEX file synchronization, image compilation, and unused DEX file cleaning are applied. In addition: allow the user to modify the timing of these optimizations.
- Zygote compression and prefork, to minimize memory fragmentation and improve app startup by having Zygote preloaded in shared memory.
- Pin ART compilation on big cores to improve batch performance by up to +20% when starting apps. If compilation occurs in the background, use only small cores, saving energy.
- Avoid using debug libartd, use production libartd and cut out debugs that only get in the way and fill applications with useless code, reducing the size of apps and providing slight space savings.
- Rest assured that we will use ART and JIT simultaneously, allowing users to take full advantage of the optimizations of both technologies. Preliminary improvements include adding JIT profiles to devices running Android 13 and lower.
- Make sure the DEX is 64bit, for ROMs that don't have this optimization.
- Reduce memory footprint and storage usage, making ART more efficient and economical depending on the environment it is placed in.
- Every ten days, if an app is not used during that period, it is considered "discarded", reducing its optimizations to save space.
- And best of all... it's Open Source! If you want to help this project with additional optimizations, tips, etc., let me know, I'd really appreciate help with this project that I made with the purpose of being fun and a way to pass the time.

### Warning!
If you use it together with my Basic Cleaner module, remember to set the same final cleaning times in the panels of this module and the basic cleaner. Don't worry, both will not run at the same time. Whereas the basic cleaner and ARTv3 when run, they will check the period between them. The first one that runs will cancel the execution of the second one because it is in the same "period".

### Credits