# subprocess
cross platform subprocess library for c++ similar to design of python subprocess.
This library expands on [this](https://github.com/benman64/subprocess) open-source library.

We made the following changes:
 - Minimised build;
 - Changed build system to Meson;
 - Added support for timeouts, i.e. `subprocess::run({'sleep', '10'}, subprocess::RunBuilder().timeout(5))`;
 - introduced backward compatibility for c++11-enabled compilers (was c++17 before)

See their [subprocess documentation](https://benman64.github.io/subprocess/index.html) for further documentation.


## requirements

- c++11 or greater
- linked with support for threading


## Usage
To use the latest released subprocess wrap version, create `<root-project>/subprojects/subprocess.wrap`, containing:
```
[wrap-git]
url = https://github.com/Sebastiaan-Alvarez-Rodriguez/subprocess
revision = v0.4.0
```

To use older releases, check the instructions in the release notes [here](https://github.com/Sebastiaan-Alvarez-Rodriguez/subprocess/releases).