
- AUR package location: <https://aur.archlinux.org/packages/sanskrit-fonts/>
- Package source code locations:
    - git clone git@github.com:sanskrit-coders/sanskrit-fonts-aur.git
    - git clone ssh://aur@aur.archlinux.org/sanskrit-fonts.git

## Creating a new Arch Linux package release
- Just update <https://github.com/sanskrit-coders/sanskrit-fonts/releases>.
- Verify package by running `makepkg -si`.
- Update AUR repository.
  - Set remote: `git remote add ssh://aur@aur.archlinux.org/dyuganga.git .`
  - Generate or update .SRCINFO with `makepkg --printsrcinfo > .SRCINFO`
  - Push to the AUR repo. (Even a single invalid commit will cause rejection.)

