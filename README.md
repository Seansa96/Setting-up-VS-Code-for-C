# Setting-up-VS-Code-for-C

check if you have gcc
	gcc --version
if you don't have it, update your repo with sudo apt update
now run sudo apt install gcc
then grab the build-essential package which should have most of the standard necessary c libraries you'll need
now get cmake, you can choose other stuff but this is what i use
sudo apt install cmake

pretty much all set, now let's go into vscode
now navigate to where you want to create your project directory, i just usally put it in my repos folder since that's where all my git
repos live

make your dir with mkdir or however you want
now you'll need your cmakelists file. this will basically give the necessary paths for cmake to track and build your program
you'll now need a build directory for cmake to operate out of. 
this is basically hwen you can actually make your project or if you already have it named, simply plug and play
mkdir build
now, you'll build your program, but you need to build it from the project directory, but you'll want to actually
stay in the build directory for running the program afterwards, so we'll just do
cmake ..
 
you'll have to do this after cleans too, which is when you get rid of any possible conflicting or corrupting values after
refactoring your code for whatever reason, so keep that in mind if you're having issues building your program

now that the architecture for building your program is in place, we can simply run the command
make
you should see the console provide feedback, for example here it'll point out possible conflicts or concerns
the executable file for your c program has been made and linked, now you just run it
./practice.c
and there's the output.  a little more involved than say python but not too bad once you understand everything involved.
