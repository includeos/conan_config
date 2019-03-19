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
To prevent overwriting any existing conan configuration the IncludeOS configuration can be tested by creating a custom conan home. To do this set the environment variable `CONAN_USER_HOME` to a path where a `.conan` folder will be created. 
