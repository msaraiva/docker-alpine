Erlang/OTP on Alpine Linux
=====

Erlang/OTP minimal environment. 

- Latest version: **18.0 (18.0.2 patch applied)**
- Image size: **16.78 MB**

See [Erlang/Elixir on Alpine Linux](https://github.com/msaraiva/alpine-erlang) to learn more about creating **minimal Erlang/Elixir docker images with Alpine Linux**.

The following packages are pre-installed:

- ncurses-libs
- erlang-kernel
- erlang-stdlib
- erlang-compiler
- erlang

> **Notice:** In order to keep images as compact as possible, Erlang libraries for Alpine Linux are split into many different packages. The full list of Erlang packages available can be found [here](http://pkgs.alpinelinux.org/packages?package=erlang%25&repo=all&arch=x86_64)

## Usage

```
$ docker run --rm -it msaraiva/erlang erl
Erlang/OTP 18 [erts-7.0.2] [source] [64-bit] [smp:4:4] [async-threads:10] [kernel-poll:false]

Eshell V7.0.2  (abort with ^G)
1> io:fwrite("Hello, world!\n").
Hello, world!
ok
2> 
```
