# Cryptorado dockerfiles

Sometimes Cryptorado needs docker images for projects which don't have any
hosted themselves, and so we have to write Dockerfiles and build/host those
images ourselves. This repo is for the collaborating on Dockerfiles and the
various build resources which go with them.

In general you should be able to run `make` in each directory to build and push the image.

## nebula

This is an image of https://github.com/slackhq/nebula.git that we use to 
create a VPN among the Cryptorado-Node IPFS cluster members.

It is built using Docker's cross-platform buildx feature, so you may need to
follow [these instructions](https://docs.docker.com/docker-for-mac/multi-arch/) to enable that on your machine.