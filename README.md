# Fling Build 

This docker compose pulls the latest version of Fling from the master branch and 
builds it with GCC and Clang. 

* `make build` : Build the docker containers
* `make run` : Compile Fling and run the unit test suite
* `make run-d` : Compile Fling and run the unit test suite detatched from the containers. 

If you want to build a specific branch in Docker, then pass the `DockerBuildFlags` 
option to `make`.

Ex: `make build-base DockerBuildFlags=debug-renderpass` will build the debug-renderpass 
branch from git. 