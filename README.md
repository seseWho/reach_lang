# reach_lang

Install and Initialize

Reach is designed to work on POSIX systems with make, Docker, and Docker Compose installed. The best way to install Docker on Mac and Windows is with Docker Desktop.2

You probably already have make installed. For example, OS X and many other POSIX systems come with make, but some versions of Linux do not include it by default and will require you to install it. If you're on Ubuntu, you can run sudo apt install make to get it.3

You'll know that you have everything installed if you can run the following three commands without errors4

 
$ make --version
 
$ docker --version
 
$ docker-compose --version
If you're using Windows, consult the guide to using Reach on Windows.5

Once you've confirmed that they are installed, choose a directory for this project. We recommend6

 
$ mkdir -p ~/reach/tut && cd ~/reach/tut
Next, download Reach by running7

 
$ curl https://docs.reach.sh/reach -o reach ; chmod +x reach
You'll know that the download worked if you can run8

 
$ ./reach version
The recommended next step, although optional, is to set up your environment with9

 
$ ./reach config
This will make subsequent uses of the reach script more convenient by tuning its runtime behavior to your specific needs and only downloading the dependencies you'll actually use.10

reach config sets overridable defaults for all Reach projects on your development machine and not just the current one, so feel free to skip this step if you'd prefer not to make your choices global.11

Since Reach is Dockerized, when you first use it, you'll need to download the images it uses. This will happen automatically when you first use it, but you can do it manually now by running12

 
$ ./reach update
You'll know that everything is in order if you can run13

 
$ ./reach compile --help

..........

This is now enough for Reach to compile and run our program. Let's try by running42

 
$ ./reach run
Reach should now build and launch a Docker container for this application. Since the application doesn't do anything, you'll just see a lot of diagnostic messages though, so that's not very exciting.43

The entire process that we just went through can be automated by running44

 
$ ./reach init
when you start your next project!