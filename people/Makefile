PEOPLE=mwitting sneumann

all: $(PEOPLE)

.PHONY: all $(PEOPLE)

%: %.png %-square.png %.ico

#ALL2: sneumann.png sneumann-square.png sneumann.ico

# PNG
%.png: %.svg
	inkscape --without-gui --file=$< --export-png=$@ --export-dpi=150

# Squaree PNG with white background 
# suitable as avatar

%-square.png: %.png
	convert -background none $< -gravity center -extent 304x304 $@

%.ico: %.png
	convert -background white $< -gravity center -extent 304x304 -resize 48x48 $@


