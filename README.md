# Item Catalog

> Dustin D'Avignon

## About

This is the fourth project for the Udacity Full Stack Nanodegree. The Item Catalog project consists of developing an application that provides a list of items within a variety of categories, as well as provide a user registration and authentication system. This project uses persistent data storage to create a RESTful web application that allows users to perform Create, Read, Update, and Delete operations.

A user does not need to be logged in in order to read the categories or items uploaded. However, users who created an item are the only users allowed to update or delete the item that they created.

This program uses third-party auth with Google or Facebook. Some of the technologies used to build this application include Flask, Bootsrap, Jinja2, and SQLite.


## Skills used for this project
- Python
- HTML
- CSS
- Bootstrap
- Flask
- Jinja2
- SQLAchemy
- OAuth
- Facebook / Google Login

## Some things you might need
- [Vagrant](https://www.vagrantup.com/)
- [Udacity Vagrantfile](https://github.com/udacity/fullstack-nanodegree-vm)
- [VirtualBox](https://www.virtualbox.org/wiki/Downloads)

## Getting Started

- Install Vagrant and VirtualBox
- Clone the Vagrantfile from the Udacity Repo
- Clone this repo into the `catlog/` directory found in the Vagrant directory
- Run `vagrant up` to run the virtual machine, then `vagrant ssh` to login to the VM
- from the main directory run `sudo pip install -r requirements`
- run application with `python application.py` from within its directory
- go to `http://localhost/categories` to access the application
- *if first time running, you must add a category before adding an item


## JSON Endpoints

`/category/JSON` - Returns JSON of all categories in catalog

<img src="screenshots/categoryJSON.png" width="1000">

`/category/<int:cid>/list/<int:mid>/JSON` - Returns JSON of selected item in category

<img src="screenshots/particularitemJSON.png" width="1000">

`/category/<int:cid>/list/JSON` - Returns JSON of all items in particular category in catalog

<img src="screenshots/jsonforparticularcategory.png" width="1000">

## Landing Page(not yet logged in)
`/category`

<img src="screenshots/landing.png" width="1000">

## Authentication(Logging in)

`/login` 

<img src="screenshots/authentication.png" width="1000">

## Landing Page(Logged in)

`/login` 

<img src="screenshots/loggedin.png" width="1000">


## Adding New Category
`/category/new` 
<img src="screenshots/newcategory.png" width="1000">

## Adding New Item
While adding info about item, in category list only those categories appear which that user has created
`'/category/item/new/`
<img src="screenshots/newItem.png" width="1000">

## Item List(not authorised)
Example of logged in but not authorised
<img src="screenshots/loggedinbutnotauthorised.png" width="1000">

## Item List(authorised)
Example of logged in & authorised
<img src="screenshots/itemslistwhenloggedinandauthorised.png" width="1000">


## Possible improvements

- Add an additional data model so that users can add Stores
- Image Upload, possible future addition with file upload
- Styling and layout could improve
- Implement CSRF protection on CRUD operations.
