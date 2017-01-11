Elixir on Alpine Linux
=====

Elixir is a dynamic, functional language designed for building scalable and maintainable applications.

Image size: **24.1 MB**

See [Erlang/Elixir on Alpine Linux](https://github.com/msaraiva/alpine-erlang) to learn more about creating **minimal Erlang/Elixir docker images with Alpine Linux**.

> **Notice:** This image does not contain git, wget, rebar or hex. If you need to download dependencies, see [msaraiva/elixir-dev](https://registry.hub.docker.com/u/msaraiva/elixir-dev/)

The following packages are pre-installed:

- erlang + dependencies
- elixir

> **Notice:** In order to keep images as compact as possible, Erlang libraries for Alpine Linux are split into many different packages. The full list of Erlang packages available can be found [here](https://pkgs.alpinelinux.org/packages?name=erlang%25&repo=all&arch=x86_64&maintainer=all)

## Usage

```
$ docker run --rm -it msaraiva/elixir iex
Erlang/OTP 18 [erts-7.3.1] [source] [64-bit] [async-threads:10] [kernel-poll:false]

Interactive Elixir (1.4.0) - press Ctrl+C to exit (type h() ENTER for help)
iex(1)> IO.puts "Hello there!"
Hello there!
:ok
iex(2)>
```
