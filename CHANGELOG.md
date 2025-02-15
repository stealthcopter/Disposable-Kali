# Changelog
All notable changes to this project will be documented in this file.

## [0.2.1]
### Added
- pkgs_exploits.sh - added more packages for ftp, smb and webdav
- shell_aliases.sh - added additional aliases
### Fixed
- change pkgs_upgrade.sh to not be silent (was killing grub)

## [0.2] - 2019-8-11
### Fixed
- Was incorrectly checking for /tmp file flags with -s, changed to -e to make scripts idempotent
- Disabled misleading colorization from vagrant with keep_color
### Changed
- Moved scripts into files in the /scripts directory so that they can be used outside of Vagrant, and better seperation for source control
- Removed timezone setting
- Remove searchsploit -u, way too slow for this (papers)
- Made adding swap space configurable
- Made UFW allow ports configurable
- Moved almost all customizations to vagrant variables
### Added
- netcat aliases to include rlwrap
- mingw aliases
- python web server alias
- fuzzbunch installer on wine (mostly working, python install is still manual)
- useful git repos cloned

## [0.1.1] - 2019-07-xx
### Fixed
- Less obnoxious header comments in Vagrantfile
- Updated README.md
- Added crude check (/tmp file) to prevent multiple appends to sshd config file
- Changed UFW to stay disabled and require explicit enabling

### Added
- Added this CHANGELOG.MD
- Added TCP 443 as a UFW rule, removed my custom ports
- Added updatedb to script_packages_extra

## [0.1.0] - 2019-06-29
### Added
- Initial release
