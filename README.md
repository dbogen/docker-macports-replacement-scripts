# boot2docker-macports-replacement-scripts
Scripts to replace Macports binaries with docker containers.

# Description
I got tired of working with Macports and was inspired by some of the docker examples floating around online.  I decided to replace my Macports installed ports with docker containers.

The goal was to replace (as seamlessly as possible) the native Macports binaries with docker containers that replicated the functionality.  I didn't want to worry about whether boot2docker was already running, nor did I want to worry about whether any particular shell had all the boot2docker environment variables loaded.

# How-To

1. Use the Dockerfiles (if necessary) to generate the relevant containers.
2. Place the scripts somewhere in your PATH.  I have them in ~/bin.
3. Execute the scripts to test your installation.

If all has gone according to plan, you should be able to execute the binaries in the docker containers just like they are native to your system.

Obviously, there are caveats.  wget, for instance, can only download into one place.  Since I always want downloaded files to end up in my Downloads directory, that limitation is fine with me.  Similarly, convert (part of ImageMagick) can only work with files located in directories mounted into the container.

Regardless, these are only examples of what you can do.  Once you understand the basic idea, you can easily adapt the scripts to replicate whatever Macport package you're trying to replace.

