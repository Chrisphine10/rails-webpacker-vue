# README

# rails-webpacker-vue
There is a lot of difficulty in using vue via the webpacker module. I hope this helps to solvve most of the errors people have been getting.

After creating the project with rails new <projectname> --webpacker=vue, you will realize that vue will be bringing some errors on the console. To fix this, follow the steps below.
	
# 1. Delete the node_modules folder from the project directory.
# 2. If you are using yarn, run:

	```
	yarn add @rails/webpacker@next
	```
else if you are using npm, run: 
	```
	npm i @rails/webpacker@next
	```
# 3. Run the code below on the terminal: 
	```
	bundle exec rails webpacker:install
	```
This is to reinstall the webpacker module and create a new node_module folder.
# 4. Run the code below on the terminal:
	```
	rails webpacker:install:vue
	```
This is to config the vue package into the webpacker module.
