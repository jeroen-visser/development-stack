# development-stack

## Installation

You can move the `bin` directory to `~/bin` and add the bin directory to you `$PATH`
```
export PATH=$HOME/bin:$PATH
```

Or you can move the `bin` files into your `/usr/local/bin/` directory

```
# Run as root
mv bin/* /usr/local/bin
```

## Usage

Export env variable `IDE_PHP_VERSION` by running or add the following command to your `~/.bashrc` or `~/.zshrc` file:

```
# For PHP 7.0
export IDE_PHP_VERSION="70"
```

```
# For PHP 7.1
export IDE_PHP_VERSION="71"
```
