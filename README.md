# Singularity

Singularity repositories.

Only supports only x86_64 and aArch64 platforms.

```conf
#user-repos.conf -> /etc/pacman.conf

[singularity]
SigLevel = PackageRequired
Server = https://wasertech.github.io/$repo/$arch
```