Elixir on Alpine Linux
=====

Elixir is a dynamic, functional language designed for building scalable and maintainable applications.

Image size: **21.75 MB**

See [Erlang/Elixir on Alpine Linux](https://github.com/msaraiva/alpine-erlang) to learn more about creating **minimal Erlang/Elixir docker images with Alpine Linux**.

> **Notice:** This image does not contain git, wget, rebar or hex. If you need to download dependencies, see [msaraiva/elixir-dev](https://registry.hub.docker.com/u/msaraiva/elixir-dev/)

The following packages are pre-installed:

- erlang + dependencies
- erlang-crypto 
- erlang-syntax-tools
- elixir

> **Notice:** In order to keep images as compact as possible, Erlang libraries for Alpine Linux are split into many different packages. The full list of Erlang packages available can be found [here](http://pkgs.alpinelinux.org/packages?package=erlang%25&repo=all&arch=x86_64)

## Usage

```
$ docker run --rm -it msaraiva/elixir iex
Erlang/OTP 18 [erts-7.0.2] [source] [64-bit] [smp:4:4] [async-threads:10] [kernel-poll:false]

Interactive Elixir (1.1.0) - press Ctrl+C to exit (type h() ENTER for help)
iex(1)> IO.puts "Hello there!"
Hello there!
:ok
iex(2)>    
```
