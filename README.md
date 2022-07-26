<p align="center">
   <img src="https://user-images.githubusercontent.com/77242216/194732352-1ea0ea50-a2c3-4aec-88d2-70d13bed3ca6.svg" height="96" >
</p>

# KALIPAK: Kali Metapackage CLI

I created this script because I didn't want to install all of Kali but I still wanted access to Kali metapackages on my current Linux distribution. Currently works on Debian for now. Ubuntu has some issues. Please use this script with caution.

> View the [Changelog](CHANGELOG.md) for project history.

### What is a Metapackage?

Metapackages are used to install many packages at once, created as a list of dependencies on other packages. Kali Linux uses these in a few ways such as allowing users to decide how many packages out of the total Kali list they would like to install. — *excerpt from [kali.org](https://www.kali.org/docs/general-use/metapackages)*

## Install & run

To install kalipak on Linux, run any of the one-liners below.

1. Using `git`:
   ```bash
   git clone https://github.com/neuralpain/kalipak /tmp/kalipak && cp -f /tmp/kalipak/kalipak /bin && chmod +x /bin/kalipak
   ```
2. Using `wget`:

   Install to `/bin` directory

      ```bash
      wget -O kalipak https://gg.gg/kalipak && chmod +x ./kalipak && sudo mv -f ./kalipak /bin
      ```

   Or download and run

      ```bash
      wget -O kalipak https://gg.gg/kalipak && chmod +x ./kalipak && ./kalipak --init
      ```

3. Or for a portable installer, download and run the [kalipak-install](kalipak-install) script (`wget` is required).

After installing kalipak, run `kalipak --init` to prepare prepare your system for working with Kali metapackages; then use the menu to select what you need. `--init` will be ignored on Kali Linux regardless so just run `kalipak` on Kali.

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

  --reset       Same as '--init' but invokes '--purge' beforehand.
  --update      Update package list and upgrade with confirmation.
  --purge       Remove sources added by KALIPAK.
  --info        Display information aout your Linux distribution.
  --version     Display version info and exit.
  --help        Display this help and exit.
```

## License

**KALIPAK** is available under the MIT License. See [LICENSE](LICENSE) for the full license text.
