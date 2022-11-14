# Singularity

Singularity repositories for aArch64.

## Navigation

- [Home](/singularity)

## Usage

Add the Singularity repository to your pacman configuration.
 
```conf
#user-repos.conf -> /etc/pacman.conf

[singularity]
SigLevel = PackageRequired
Server = https://wasertech.github.io/$repo/$arch
```
Recive my public GPG key.

```zsh
❯ sudo pacman-key --recv-keys 6D8A4B5865E71713
gpg: clef 6D8A4B5865E71713 : clef publique « Danny Waser (Waser Technologies) <waser@waser.tech> » importée
gpg:       Quantité totale traitée : 1
gpg:                     importées : 1
```
Sign my key to approve it.

```zsh
❯ sudo pacman-key --lsign-key 6D8A4B5865E71713
```
You can now update pacman db.

```zsh
❯ sudo pacman -Syyu
:: Synchronisation des bases de données de paquets…
 core                  164.5 KiB  1266 KiB/s 00:00 [######################] 100%
 extra                1864.6 KiB  3.91 MiB/s 00:00 [######################] 100%
 community               7.1 MiB  3.87 MiB/s 00:02 [######################] 100%
 multilib              175.6 KiB  3.43 MiB/s 00:00 [######################] 100%
 singularity             5.2 KiB  27.1 KiB/s 00:00 [######################] 100%
:: Début de la mise à jour complète du système…
 il n’y a rien à faire
```
