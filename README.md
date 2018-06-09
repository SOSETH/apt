# Role: apt
Configuration of package management tools.

## Settings
| Name | Default value | Description |
| ---- | ------------- | ----------- |
| `apt_install_extra` | `False` | Install extra APT tools (apt-files and apt-listchanges) |
| `apt_with_backports` | `False` | Whether to enable backports (Debian) |
| `apt_add_custom_repo` | `False` | Add a custom APT repository (see below)? |
| `apt_custom_repo_url` | | URL of the custom repository to add |
| `apt_custom_repo_key` | | Key _data_ (starts with BEGIN PGP PUBLIC...) of the key used to sign the custom repository |
| `apt_default_mirror` | `http://debian.ethz.ch/debian/` | Default debian mirror |
| `apt_security_mirror` | `http://security.debian.org` | Default debian security mirror |
| `apt_ubuntu_mirror` | `http://ubuntu.ethz.ch/ubuntu/` | Default ubuntu mirror |
| `apt_ubuntu_security_mirror` | `http://security.ubuntu.com/ubuntu/` | Default ubuntu security mirror |
| `apt_add_src` | `False` | Whether to add source repositories |
| `apt_is_special_snowflake` | `False` | If set, do not apply main config. Useful for debian forks (e.g. Raspbian)
| `apt_debian_package_types` | `main contrib non-free` | Repo sections to add for debian |
| `apt_ubuntu_package_types` | `main universe multiverse` | Repo sections to add for ubuntu |
