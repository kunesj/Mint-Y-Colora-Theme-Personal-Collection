My personal Mint-Y-Colora Themes
================================

Build some themes for current vesion of Cinnamon, since Mint-Y-Colora-Theme-Collection repo is outdated.

Using:

	https://github.com/linuxmint/mint-themes
	https://github.com/HattDroid/Mint-Y-Colora-Theme

Build date: 2018-11-10

Script fix
----------
Script I used left some default colors behind, so I needed to edit "1-change-color.sh" to replace: 
```
find $SRC_DIR -name "*.*" -type f -exec sed -i 's/'$oldcolour1'/'$newcolour1'/g' {}  \;
find $SRC_DIR -name "*.*" -type f -exec sed -i 's/'$oldcolour2'/'$newcolour2'/g' {}  \;
find $SRC_DIR -name "*.*" -type f -exec sed -i 's/'$oldcolour3'/'$newcolour3'/g' {}  \;
find $SRC_DIR -name "*.*" -type f -exec sed -i 's/'$oldcolour4'/'$newcolour4'/g' {}  \;
find $SRC_DIR -name "*.*" -type f -exec sed -i 's/'$oldcolour5'/'$newcolour5'/g' {}  \;
find $SRC_DIR -name "*.*" -type f -exec sed -i 's/'$oldcolour6'/'$newcolour6'/g' {}  \;
find $SRC_DIR -name "*.*" -type f -exec sed -i 's/'$oldcolour7'/'$newcolour7'/g' {} \;
```
with:
```
find $SRC_DIR -type f -exec sed -i 's/'$oldcolour1'/'$newcolour1'/g' {}  \;
find $SRC_DIR -type f -exec sed -i 's/'$oldcolour2'/'$newcolour2'/g' {}  \;
find $SRC_DIR -type f -exec sed -i 's/'$oldcolour3'/'$newcolour3'/g' {}  \;
find $SRC_DIR -type f -exec sed -i 's/'$oldcolour4'/'$newcolour4'/g' {}  \;
find $SRC_DIR -type f -exec sed -i 's/'$oldcolour5'/'$newcolour5'/g' {}  \;
find $SRC_DIR -type f -exec sed -i 's/'$oldcolour6'/'$newcolour6'/g' {}  \;
find $SRC_DIR -type f -exec sed -i 's/'$oldcolour7'/'$newcolour7'/g' {} \;
```
Some colors in xfwm4 are still left as default, but I have no clue why they are not replaced...

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


