My personal Mint-Y-Colora Themes
================================

Build some themes for current vesion of Cinnamon(3.8.9) included in Linux Mint 19, since both original Mint-Y-Colora-Theme-Collection and Mint-Y-Colora repos are outdated.

Used repos:

	https://github.com/linuxmint/mint-themes
	https://github.com/kunesj/Mint-Y-Colora-Theme

Build date: 2018-11-17

How to do this yourself
-----------------------

1. Prepare code and data for theme generation
```
git clone https://github.com/linuxmint/mint-themes.git
git clone https://github.com/kunesj/Mint-Y-Colora-Theme.git
cp Mint-Y-Colora-Theme/*.sh mint-themes/
cp Mint-Y-Colora-Theme/*.py mint-themes/
cd mint-themes/
./0-install-tools.sh
```

2. Choose theme colors (in `autobuild-themes.py`)
```
'Numix': {'light': 'd64937', 'dark': 'd64937'},
```

3. Generate theme(s)
```
./autobuild-themes.py
```
Build themes will be put into `~/.themes`

Used colors
-----------
```
## Monochrome

Mint-Y-Smoke
personallightcolour=A1A1A1
personaldarkcolour=A1A1A1

Mint-Y-Majestic
personallightcolour=5F5F5F
personaldarkcolour=5F5F5F

## Numix

Mint-Y-Numix (Correct color version)
personallightcolour=d64937
personaldarkcolour=d64937

Mint-Y-Numix-Orange (Mint-Y-Colora-Theme-Collection version)
personallightcolour=FFA726
personaldarkcolour=FFA726
```
More colors from Mint-Y-Colora-Theme-Collection can be found in it's repo in:
```
Mint-Y-*/cinnamon/cinnamon.css
	.cinnamon-link { color: personaldarkcolour }
	.cinnamon-link:hover { color: personallightcolour }
```


