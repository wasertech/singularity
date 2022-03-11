# Singularity

Singularity repositories.

Supports only x86_64 and aArch64 platforms for now.

```conf
#user-repos.conf -> /etc/pacman.conf

[singularity]
SigLevel = PackageRequired
Server = https://wasertech.github.io/$repo/$arch
```