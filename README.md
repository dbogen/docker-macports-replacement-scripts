# docker-macports-replacement-scripts
Scripts to replace Macports binaries with docker containers.

# Description
I got tired of working with Macports and was inspired by some of the docker examples floating around online.  I decided to replace my Macports installed ports with docker containers.

The goal was to replace (as seamlessly as possible) the native Macports binaries with docker containers that replicated the functionality.  I didn't want to worry about whether docker-machine was already running, nor did I want to worry about whether any particular shell had all the docker-machine environment variables loaded.

Regardless, these are only examples of what you can do.  Once you understand the basic idea, you can easily adapt the scripts to replicate whatever Macport package you're trying to replace.

# How-To

1. You'll need to download and install [Docker Toolbox](https://www.docker.com/toolbox).
1. Use the Dockerfiles (if necessary) to generate the relevant containers.
2. Place the scripts somewhere in your PATH.  I have them in ~/bin.
3. Execute the scripts to test your installation.

If all has gone according to plan, you should be able to execute the binaries in the docker containers just like they are native to your system.

# Caveats and Assumptions

## Caveats 
wget, for instance, can only download into one place.  Since I always want downloaded files to end up in my Downloads directory, that limitation is fine with me.  

convert (part of ImageMagick) can only work with files located in directories mounted into the container.

## Assumptions

The scripts assume that the docker-machine-functions file is located in the same directory as themselves.

The functions file assumes that your docker-machine image is named default.  If that is not true, you'll have to change it in the functions file.

The functions file also assumes that your docker-machine image uses virtualbox as the driver.  If that is not true, you'll need to change it in the functions file.

# Comments and concernts

For comments and concerns, you can contact me via GitHub or on [Twitter](https://twitter.com/d_bogen).
