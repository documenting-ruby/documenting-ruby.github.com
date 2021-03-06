---
layout: post
title: "List of Undocumented Areas"
tags: 
  - help
---

Many modules in Ruby lack a basic top-level description of what they do. In many cases, this is a relatively easy task to do. What is needed is one or two paragraphs of description, and a couple of realistic examples of its use.

### Example of well documented classes

  - [OpenSSL](https://github.com/documenting-ruby/ruby/blob/325a50fc572516a171d640765d6ddf9b20be14dc/ext/openssl/ossl.c#L555-L1035)
  - [BasicObject](https://github.com/documenting-ruby/ruby/blob/6964df9a21633be9c77eba96e56f8a62db8901d1/object.c#L3185-L3236)

### Classes/Modules which lack documentation

  -  Debug
  -  Fiddle
  -  Profile, Profiler
  -  RSS
  -  RbConfig

### Classes/Modules with poor documentation

  - ARGF
  - Digest: no examples (Digest::MD5 is not even in the class list)
  - OptionParser
  - Racc
  - Rinda
  - Sync, Sync_m
  - ZLib

### More specialized things

  - initialize_copy

<a name="CoverageReport"></a>
<a class="top" href="#">top</a>
### Undocumented Coverage Report

We also have a report of undocumented modules, classes, and methods that was
generated from RDoc using the `rdoc -C path/to/files` command.

* <a href="/assets/undocumented_core.txt">Core classes</a>
* <a href="/assets/undocumented_lib.txt">Standard Ruby libraries</a>
* <a href="/assets/undocumented_ext.txt">Standard Ruby extensions</a>

### Some other tips for finding areas to document

  - Look near `Init_<class name>` in `<class_name>.c`
