# Changelog

## 1.3.1

- Add `--purge` flag to remove sources and `--reset` flag to remove sources and *then* initialize. This was added for quick access rather than runing kalipak and navigating the menu for these options.
- Fix `GPG` signature verification error.
- Improve messages from kalipak.
- Code optimization and minor bug fixes.
- Update `README.md`.

## 1.3.0

- Add `KALIPAK_Init` to compose the stepwise refinement of the initializing code (for installing keys and mirrors) after functional decomposition.
- Add `--init` flag to initialize kalipak.
- Add support for installing `GPG` keys for package verification.
- Add timer `StartSession`, `EndSession`.
- Add `--info` flag to display distro information.
- Add support for retrieving distro name.
- Add support for adding Kali sources in `/etc/apt/sources.list.d`.
- Bug fixes and improvements.

## 1.2.1

- Code optimization and improvements.
- Updated `README.md`.

## 1.2.0

- Add support for updating packages in the menu or with `kalipak -i` before the menu is displayed.
- The `PackageSelect` function has been renamed to `SelectPackage`.
- Minor improvements.
- Updated `README.md`.

## 1.1.0

- Code optimization.

## 1.0.0

- Initial release of kalipak.
