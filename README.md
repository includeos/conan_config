# Conan configuration

This repository contains conan settings used by IncludeOS.

Using `conan config install` this repository configures:

- The conan bintray remotes for [IncludeOS](https://github.com/hioa-cs/IncludeOS):

- The profiles we have in the [profiles directory](profiles/README.md)


To configure your system for IncludeOS do:
```
$ conan config install https://github.com/includeos/conan_config.git
```

## Using multiple conan configurations
To prevent overwriting any existing conan configuration the IncludeOS
configuration can be tested by creating a custom conan home.
To do this set the environment variable `CONAN_USER_HOME` to a path where a
`.conan` folder will be created.


### Profiles in Support

The profiles directory contains a list of profiles that we currently use in the
development and testing of [IncludeOS](https://github.com/includeos/includeos).
Below is a list of profiles with description.

#### Build on MacOS

__Clang 6.0 :__

- clang-6.0-macos-x86_64

#### Build toolchain for MacOS

- apple-clang-10-macos-toolchain

#### Build on Linux

__Clang 6.0 :__

- clang-6.0-linux-x86_64-toolchain
- clang-6.0-linux-x86_64

For building on `x86_64` for `x86` use the profiles below:

- clang-6.0-linux-x86-toolchain    
- clang-6.0-linux-x86

__GCC 7.3 :__

- gcc-7.3.0-linux-x86_64-toolchain
- gcc-7.3.0-linux-x86_64
- gcc-7.3.0-linux-aarch64-toolchain
- gcc-7.3.0-linux-aarch64               

__GCC 8.2 :__

Currently in progress is work on `aarch64` with `gcc8.2`

- gcc-8.2.0-linux-aarch64-toolchain
- gcc-8.2.0-linux-aarch64               
