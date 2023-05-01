build:
		hugo

clean:	# Cleanup the content of the directory dist/
		rm -r dist/*

post:	
		hugo new posts/$(POST_NAME).md
		sed -i 's/title: .*/title:"$(POST_TITLE)"/' content/posts/$(POST_NAME).md
