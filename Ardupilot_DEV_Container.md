## Setup
```shell
podman run -dit --name ardupilot -v /home/host_computer/ardupilot:/ardupilot:z --userns=keep-id ubuntu
```

### exec as root and prepare
attach as root
```shell
podman exec -it --user root ardupilot bash
```

```shell
apt update
apt install passwd sudo

passwd root
passwd ubuntu

usermod -aG sudo ubuntu # or - adduser ubuntu sudo
# and exit
exit
```

```shell
podman stop ardupilot
```

## And now you can do
```shell
podman start -ai ardupilot # -ai is to attach to the terminal of the container
su ubuntu # to get the full login session
cd /ardupilot
```
now you can start to delvelop as usual