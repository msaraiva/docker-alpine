Erlang/OTP development on Alpine Linux
=====

Erlang/OTP development environment.

Latest version: **18.1**
Image size: **22.37 MB**

See [Erlang/Elixir on Alpine Linux](https://github.com/msaraiva/alpine-erlang) to learn more about creating **minimal Erlang/Elixir docker images with Alpine Linux**.

The following packages are pre-installed:

- ncurses-libs
- erlang-kernel
- erlang-stdlib
- erlang-compiler
- erlang
- erlang-dev
- erlang-reltool

> **Notice:** In order to keep images as compact as possible, Erlang libraries for Alpine Linux are split into many different packages. The full list of Erlang packages available can be found [here](http://pkgs.alpinelinux.org/packages?package=erlang%25&repo=all&arch=x86_64)

## Usage

```
$ docker run --rm -it msaraiva/erlang-dev erl
Erlang/OTP 18 [erts-7.1] [source] [64-bit] [smp:4:4] [async-threads:10] [kernel-poll:false]

Eshell V7.1  (abort with ^G)
1> io:fwrite("Hello, world!\n").
Hello, world!
ok
2>
```
