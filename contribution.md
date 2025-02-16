---
layout: default
title: Contributing to Rspamd
---

# Contributing to Rspamd

Rspamd is an open-source software distributed under the terms of permissive [Apache license](LICENSE.txt). To contribute to rspamd you might want to go to the [GitHub project page](https://github.com/rspamd/rspamd), study the current issues and suggest solutions.


## Ideas list

Here is a short summary of these ideas.

### Rspamd documentation improvements

Many rspamd modules are undocumented. We would appreciate any help in documenting them in markdown format for this site.

* Difficulty: easy
* Required skills: markdown, ability to read code in lua
* Desire: high

### Rspamd Lua API improvements

The original Lua bindings are too complicated at the moment. The idea is to unify its arguments by using indexed tables and to use FFI bindings for calling of C code.

* Difficulty: medium
* Required skills: C and Lua knowledge
* Desire: high

### Additional statistics backends

Currently, we support plain memory-mapped files only for storing statistics tokens. However, we'd like to support other backends, such as redis, sqlite or other storages.

* Difficulty: hard
* Required skills: C
* Desire: high

### Flexible event reactors support

So far, rspamd works with libevent only, however, supporting of other event reactors, such as libev, libuv or picoevent would be interesting.

* Difficulty: medium
* Required skills: C
* Desire: medium

### Interaction with GeoIP

For some checks, it is good to check geographical location of the sender. Rspamd now supports radix tries and it is possible to write geoip plugin completely in lua therefore.

* Difficulty: easy
* Required skills: Lua
* Desire: medium

### Better debugging support

Currently, rspamd allows to turn on and turn off debugging logs globally. Ideally, we would like to have a fine-grained set of modules to enable or disable debugging. Moreover, many places in rspamd code lack debugging support, which is a problem when dealing with bugs.

* Difficulty: hard
* Required skills: C
* Desire: medium

### New rules

The never-ending task of writing new rules is here. Spam fighting is a continuous process, so we need help from mail administrators who want to contribute their useful rules.

* Difficulty: easy
* Required skills: Lua
* Desire: high

### Rewriting lua plugins and rules in a more structured and functional style

With introducing of [lua-functional](https://github.com/rtsisyk/luafun) we want to improve the style and safety of the existing lua plugins.

* Difficulty: easy
* Required skills: Lua
* Desire: low
