# Golang Version Manager
_gvm_ is an attempt to manage multiple active golang versions.

## Installation

To install `gvm`, you can run the install script using curl:

```
curl -o- https://raw.githubusercontent.com/devzer01/gvm/install-latest/install.sh | bash
```
or wget:
```
wget -qO- https://raw.githubusercontent.com/devzer01/gvm/install-latest/install.sh | bash
```
<sub>The script clones the gvm repository to `~/.gvm` and adds the source line to your profile (`~/.bash_profile`, `~/.zshrc`, `~/.profile`, and `~/.bashrc`).</sub>

**Note:** `gvm` does not support Windows.

## Usage

```
gvm --help                      Show this message
gvm --version                   Print out the installed version of gvm
gvm install <version>           Download and install a <version>
gvm uninstall <version>         Uninstall a <version>
gvm use <version>               Modify PATH to use <version>
gvm current                     Display currently activated version
gvm ls                          List installed versions
gvm releases [filter]           Display available release versions to install, optionally filter by major and minor version ex: gvm releases 1.12 would only return 1.12.* releases
gvm flush                       Remove the cache file used in gvm releases
```

Examples:
```
gvm install 1.11.0               Install a specific version number
gvm uninstall 1.11.0             Uninstall a specific version number
gvm use 1.11.0                   Use a specific version number
```

## Contributing

Feel free to raise pull request, if you have any suggestion or improvement.

### Special Thanks
`gvm` has been inspired by [nvm](!https://github.com/creationix/nvm). Special thanks to `nvm`'s author [creationx](!https://github.com/creationix).
