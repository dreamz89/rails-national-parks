# National Parks

Beginning with the first Tree Planting Campaign in 1963, At National Parks Board (NParks) has come a long way in greening up our island city, with 4 nature reserves and more than 300 parks sprawled across Singapore to date and still growing.  

Let's create an app to showcase these wonderful parks.

# Getting Started

*   Fork and clone this repository
*   Follow the recommended process for creating your Rails app.

# Components

### Models

*   A `Park` model that stores the following attributes. Choose the appropriate data types for each (`string` or `text`)
*   `name`
*   `description`
*   `picture` (for now, have this store a URL to a picture of a park)

### Controllers

*   A controller for your home page
*   A controller for your `Park` model

### Routes and Views

| route             | description                    | controller | action/view      |
| ----------------- | ------------------------------ | ---------- | ---------------- |
| GET /             | Your home page                 | home       | index            |
| GET /parks        | list all parks                 | parks      | index            |
| GET /parks/new    | show add park form             | parks      | new              |
| POST /parks       | create park                    | parks      | create (no view) |
| GET /parks/1      | list park (id=1)               | parks      | show             |
| GET /parks/2/edit | show edit park form (id=2)     | parks      | edit             |
| PUT /parks/3      | update an existing park (id=3) | parks      | update (no view) |
| DELETE /parks/3   | delete an existing park (id=3) | parks      | destroy (no view)|

**Remember:** you can list all routes by running `rails routes` at the command line.

# Recommended Process

### Create basic app

*   Fork and clone this repo
*   cd into the directory
*   Create app `rails new ./ -T -d postgresql`
*   Create database `rails db:create`
*   Test app
*   Run server `rails s`

### Build specific functionality

*   Create model `rails g model ...` (you write the rest of this command)
*   Migrate `rails db:migrate`
*   Test models
*   run console `rails c`
*   Try some stuff...
    *   `Park.all`
    *   `Park.create`
    *   `Park.new`
    *   `Park.find`
*   Create functionality
*   Add routes to `routes.rb`. Use `resources` to create a set of RESTful CRUD routes
*   Add controllers, actions, and views where appropriate
*   Add functionality for each controller action
*   Test as needed

## Bonuses

*   Create a seed file to load some National Parks
*   Replace the URL links with Cloudinary uploads.
*   [Cloudinary Gem](https://github.com/cloudinary/cloudinary_gem)
*   [Cloudinary Upload Notes](https://wdi_sea.gitbooks.io/notes/content/06-ruby-rails/additional-topics/rails-cloudinary/readme.html)

---

## Licensing
1.  All content is licensed under a CC-BY-NC-SA 4.0 license.
2.  All software code is licensed under GNU GPLv3. For commercial use or alternative licensing, please contact legal@ga.co.
