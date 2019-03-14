# Conan Configurations

This repository contains conan settings required for IncludeOS.

Using `conan config install` this repository configures:

- The conan bintray remote for [IncludeOS](https://github.com/hioa-cs/IncludeOS):

 https://api.bintray.com/conan/includeos/test-packages

- The profiles we have in the [profiles directory](profiles/README.md)

To configure your system for IncludeOS do:

```
  $ conan config install https://github.com/includeos/conan_config.git
```
