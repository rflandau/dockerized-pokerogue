# dockerized-pokerogue
Just a containerized version of [PokeRogue](https://github.com/pagefaultgames/pokerogue).

# Running

Just pull the image with `docker pull rflandau/pokerogue` and run it with `docker run -p 8000:8000 rflandau/pokerogue`.

If you want a more recent version of PokeRogue, see [building](#building) below.

# Building

Build this with `docker build -f Dockerfile_PokeRogue -t <username>/pokerogue .`; the build process will select for the most recent version on the default (*beta*) branch and create a container for it.

# Saves
As PokeRogue is browser-based, your save file is still hosted within your browser. This is a boon in that we don't need to deal with docker volumes, but a bane in that you will need to manually import your [pokerogue.net](pokerogue.net) save as the url will not match.
