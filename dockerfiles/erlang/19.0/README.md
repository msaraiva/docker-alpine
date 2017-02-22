Erlang/OTP on Alpine Linux
=====

Erlang/OTP minimal environment.

Latest version: **19.0**
Image size: **17.8 MB**

See [Erlang/Elixir on Alpine Linux](https://github.com/msaraiva/alpine-erlang) to learn more about creating **minimal Erlang/Elixir docker images with Alpine Linux**.

The following packages are pre-installed:

- ncurses-libs
- erlang-kernel
- erlang-stdlib
- erlang-compiler
- erlang

> **Notice:** In order to keep images as compact as possible, Erlang libraries for Alpine Linux are split into many different packages. The full list of Erlang packages available can be found [here](https://pkgs.alpinelinux.org/packages?name=erlang%25&repo=all&arch=x86_64&maintainer=all)

## Usage

```
$ docker run --rm -it msaraiva/erlang erl
Erlang/OTP 19 [erts-8.1] [source] [64-bit] [smp:2:2] [async-threads:10] [kernel-poll:false]

Eshell V8.1  (abort with ^G)
1> io:fwrite("Hello, world!\n").
Hello, world!
ok
2>
```
