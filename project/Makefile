ALL: metclassnet.png metclassnet-square.png metclassnet.ico

# PNG
metclassnet.png: metclassnet.svg
	inkscape --without-gui --file=metclassnet.svg --export-png=metclassnet.png --export-dpi=150

# Squaree PNG with white background 
# suitable as avatar

metclassnet-square.png: metclassnet.png
	convert -background none metclassnet.png -gravity center -extent 304x304 metclassnet-square.png

metclassnet.ico: metclassnet.png
	convert -background white metclassnet.png -gravity center -extent 304x304 -resize 48x48 metclassnet.ico


