build: ## Generate the website.
	hugo
clean: ## Cleanup the content of the directory dist.
	rm -r dist
post: ## Create a new blog post.
	hugo new posts/$(POST_NAME).md
	sed -i 's/title.*/title: $(POST_TITLE)/' content/posts/$(POST_NAME).md
help: ## Show this help usage
	@grep -E '^[a-zA-Z0-9_-]+:.*?## .*$$' $(MAKEFILE_LIST) | sed -n 's/^\(.*\): \(.*\)##\(.*\)/\1\3/p' | column -t  -s ' '
