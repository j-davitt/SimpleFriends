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
