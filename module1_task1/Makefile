build:
	hugo new site --force .
	git submodule add https://github.com/theNewDynamic/gohugo-theme-ananke themes/ananke
	echo "theme = 'ananke'" >> config.toml
clean:
	rm -r dist
post:
	hugo new posts/$(POST_NAME).md
	echo "title: '$(POST_TITLE)'" >> $(POST_NAME).md
