ALL: sneumann.png sneumann-square.png sneumann.ico

# PNG
sneumann.png: sneumann.svg
	inkscape --without-gui --file=sneumann.svg --export-png=sneumann.png --export-dpi=150

# Squaree PNG with white background 
# suitable as avatar

sneumann-square.png: sneumann.png
	convert -background none sneumann.png -gravity center -extent 304x304 sneumann-square.png

sneumann.ico: sneumann.png
	convert -background white sneumann.png -gravity center -extent 304x304 -resize 48x48 sneumann.ico


