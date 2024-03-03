# README

Following tutorial [here](https://www.youtube.com/watch?v=fmyvWz5TUWg)

Commands:

`rails s` starts the server

`rails g` generator command

`rails g scaffold` generates a db table
> `rails g scaffold friends first_name:string last_name:string` generates a db table named friends that has a first_name property and last_name property that are both string types.

`rails db:migrate` pushes migration into db to 'make it live' and create schema.

`bundle install` generally used to install gems that are in gemfile.

`rails routes` shows all the routes for the application

`rails g migration add_user_id_to_friends user_id:integer:index` adds a user_id property to friends table that is an integer and given an index

embedded ruby can be done on the page or referenced from controller.
> `<% %>` is used for code that doesnt get rendered to page. `<%= %>` renders to page.

Web Hosting: Heroku supports rails projects (no longer have free tier?).
>Heroku CLI is useful
Convert to postgres from sqlite3 for heroku.

In Gemfile:

- Move sqlite3 gem into development group.
- Create production group and include postgres gem.

> `group :production do`

> `gem 'pg', '~> 1.2', '>=1.2.3'` (version can differ)

> `end`

Dont forget to bundle install. `bundle install --without production` will keep the development environment on your machine so you are not getting the gems that heroku needs that might cause issues with your local machine.
