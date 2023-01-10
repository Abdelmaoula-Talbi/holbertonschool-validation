build:
	@hugo
clean:
	rm -r dist
post:
	hugo new posts/$(POST_NAME).md
	echo "title: '$(POST_TITLE)'" >> $(POST_NAME).md
