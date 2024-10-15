.PHONY: optimise_jpg optimise_png

install:
	brew install jpegoptim
	brew install pngquant

optimise_jpg:
	jpegoptim --strip-all --max=80 *.jpg

optimise_png:
	find . -name "*.png"  -mindepth 1 -maxdepth 1 -exec pngquant --quality=65-80 --strip --force --ext .png {} \;

optimise: optimise_jpg optimise_png