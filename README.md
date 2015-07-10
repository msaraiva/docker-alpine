Dockerfiles for Alpine Linux
=====

Alpine Linux is a lightweight Linux distribution built around **musl** libc and **busybox**.
The main focus of this distribution is security, simplicity and resource efficiency.
All that makes Alpine Linux perfect to work as base images for linux **containers**.

### Minimal docker images

When creating a docker image, you probably want to minimize its size as much as possible. At the same time, you might want to have access to a full-featured package system with a large range of packages available. As far as I can see, Alpine Linux is the best choice for that.

### How minimal?

```
REPOSITORY                     TAG      IMAGE ID       CREATED           VIRTUAL SIZE
msaraiva/erlang                18.0     afe36ddc5624   58 minutes ago    16.78 MB

```

See [Erlang/Elixir on Alpine Linux](https://github.com/msaraiva/alpine-erlang) to learn more about creating **Minimal Erlang/Elixir docker images with Alpine Linux**.
