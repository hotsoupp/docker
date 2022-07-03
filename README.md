# Introduction

This Repo will be housing templates used for either with or without Portainer.


## NFS-MEDIASTACK

This stack is used to spin up the following services and connect them to the requiered NFS shares. 

* Radarr
* Sonarr
* Bazarr
* SabNZBD
* Prowlarr
* Overseerr
* Tautulli

Your type of media might vary if for example you don't have any Anime, you can remove the line in the nfs-mediastack.env where it says ANIME_PATH= and remove the volumes in nfs-mediastack.yaml. 


DATADIR=            # The Directory on your local host to store the data of containers
<br>
PUID=               # User ID to run docker with
<br>
PGID=               # Group that has access to Docker
<br>
TZ=                 # Timezone of country the service is being hosted in, example Europe\Amsterdam
<br>
STORAGE_HOST=       # The IPv4 of the machine hosting your fils, Example (192.168.178.43)
MOVIES_PATH=        # The NFS path to your Movies folder, example /mnt/user/movies
TV_PATH=            # The NFS path to your Tv shows folder, example /mnt/user/Tv
ANIME_PATH=         # The NFS path to your Anime folder, example /mnt/user/anime
DOWNLOADS_PATH=     # The NFS path to your Downloads folder, example /mnt/user/downloads

