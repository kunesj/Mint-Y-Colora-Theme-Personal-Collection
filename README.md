My personal Mint-Y-Colora Themes
================================

I build some themes for current version of Cinnamon(3.8.9) included in Linux Mint 19, because both original Mint-Y-Colora-Theme-Collection and Mint-Y-Colora repos are outdated.

Used repos:

	https://github.com/linuxmint/mint-themes
	https://github.com/kunesj/Mint-Y-Colora-Theme

Build date: 2018-11-17


Installation
------------

1. Download this repository

2. Move theme folders to your `~/.themes` folder

    - `~/.themes` folder is a hidden folder

    - Make sure you copy all versions of you choosen theme (normal, dark, darker)


How to build themes yourself
----------------------------

1. Prepare code and data for theme generation
```
git clone https://github.com/linuxmint/mint-themes.git
git clone https://github.com/kunesj/Mint-Y-Colora-Theme.git
cp Mint-Y-Colora-Theme/*.sh mint-themes/
cp Mint-Y-Colora-Theme/*.py mint-themes/
cd mint-themes/
./0-install-tools.sh
```

2. Define theme colors (in `themes.json`)
```
{
    "Smoke": {"light": "A1A1A1", "dark": "A1A1A1"},
    "Majestic": {"light": "5F5F5F", "dark": "5F5F5F"}
}
```
Last line must NOT have `,` at the end!

3. Generate theme(s)
```
./autobuild-themes.py
```
Build themes will be put into `~/.themes` by default

For more details read README in `Mint-Y-Colora-Theme` repo.


Used colors
-----------
Used theme colors are located in file `themes.json`.

Most colors are taken from old `Mint-Y-Colora-Theme-Collection`, by looking at these lines:
```
Mint-Y-*/cinnamon/cinnamon.css
	.cinnamon-link { color: personaldarkcolour }
	.cinnamon-link:hover { color: personallightcolour }
```

`Mint-Y-Numix` theme from old `Mint-Y-Colora-Theme-Collection` was renamed to `Mint-Y-Numix-Orange` and replaced by my own version.
I have done this because it's colors are different from old verson of Numix theme I was using for last 4 years.
Deal with it.
