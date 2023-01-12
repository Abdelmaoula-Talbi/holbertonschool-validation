build: ## Generate the website.
	hugo
clean: ## Cleanup the content of the directory dist.
	rm -r dist
post: ## Create a new blog post.
	hugo new posts/$(POST_NAME).md
	sed -i 's/title.*/title: $(POST_TITLE)/' content/posts/$(POST_NAME).md
help: ## usage: Show this help usage
	@echo "Usage:"
	cat Makefile | grep '##' | tr -d '##'
