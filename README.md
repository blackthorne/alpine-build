# alpine-build
A lightweight docker container with dev tools for building software to run on alpine.

# build
docker build -t alpine-build .

# run
You can simply run this with something like that should work for both compiling and debugging things under alpine:
docker run --rm -it --cap-add=SYS_PTRACE -v $PWD:/dropbox alpine-build
