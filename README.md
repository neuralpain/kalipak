<p align="center">
   <img src="https://user-images.githubusercontent.com/77242216/192156018-6c07bf52-5f00-492c-b06c-34c650fcdbdd.svg" height="96" >
</p>

# KALIPAK: Kali Metapackage CLI

I created this script because I didn't want to install all of Kali but I still wanted access to Kali metapackages on my current Linux distribution. Currently works on Debian for now. Ubuntu has some issues. Please use this script with caution.

> View the [Changelog](CHANGELOG.md) for project history.

### What is a Metapackage?

Metapackages are used to install many packages at once, created as a list of dependencies on other packages. Kali Linux uses these in a few ways such as allowing users to decide how many packages out of the total Kali list they would like to install. — *excerpt from [kali.org](https://www.kali.org/docs/general-use/metapackages)*

## Install & run

To install kalipak on Linux, run the code below in order.

   ```bash
   git clone https://github.com/neuralpain/kalipak /tmp/kalipak
   sudo cp -f /tmp/kalipak/kalipak /bin
   chmod +x /bin/kalipak
   ```

After installing kalipak, run `kalipak --init` to prepare prepare your system for working with Kali metapackages. Afterwhich, use the menu to select what you need. However, if running on Kali Linux, do not use `--init`, just run `kalipak`.

## Usage

```
┌─KALIPAK─┐
Install Kali metapackages on your Linux distribution.

    kalipak [OPTION]

OPTIONS
  --init        This command will prepare your system for
                use with KALIPAK by installing required packages
                and keys for Kali certificate verification
                and should be run the first time you use KALIPAK.

  --reset        Same as '--init' but invokes '--purge' beforehand.
  --update       Update package list and upgrade with confirmation.
  --purge        Remove sources added by KALIPAK.
  --info         Display information aout your Linux distribution.
  --version      Display version info and exit.
  --help         Display this help and exit.
```

## License

**KALIPAK** is available under the MIT License. See [LICENSE](LICENSE) for the full license text.
