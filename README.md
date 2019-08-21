# Getting started with Phrase and Github - Ruby on Rails example
This Repository provides examples on how to use Phrase in general and the integration with github.

# What we want to achieve
- You will run a simple app on your machine
- You will learn how to internationalize the app
- You will learn how to integrate Phrase

# [System setup and first steps](https://vimeo.com/352687293/3ea2ac3a1a)
## Installation of necesary tools
- [Sublime - Texteditor](https://www.sublimetext.com/)
- [Homebrew - Packagemanager for Linux/MacOs](https://brew.sh/)
- Install git with homebrew with -> `$brew install git`
- Install gpg with homebrew with -> `$brew install gpg`
- [RVM -Ruby Version manager](https://rvm.io/)
  - If you run into problems with installing rvm espaicially with the
    GPG Keys, please follow the security instructions on the rvm page
- Install the right Ruby version with rvm with ->` $rvm install 2.4.1`


# Run the Application on your machine

## Get the Source code
1. Create a folder in the Terminal on your Desktop
    * ` $cd Desktop`
    * `$mkdir phrase_playground`

2. Navigate into the folder
    * `$cd phrase_playground`

3. Clone the Lunchroulette Repo from Github
    * `$git clone https://github.com/docstun/lunchroulette.git`

## Get the Webapp up and running
### Setup the enviromente for the App

1. Install Bundler -> Dependency Manger for Ruby on Rails
    * `$gem install bundler`
2. Install all gems
    * `$bundle install`

### Get the App running

1. Initialize the Database
    * `$rails db:setup`

2. Start the Server
    * `rails server`

3. [Open App in your browser](http://localhost:3000)


# Short indroduction to the Ruby on Rails enviromente
> For a short introduction to the Ruby on Rails structure, please view the
> short [video](https://vimeo.com/352687324/fc6c93f613) we provided.
> [For a deeper introduction of Ruby on Rails structure we suggested
this video](https://gorails.com/episodes/rails-application-structure)


# Localizing the App
> [Introduction to i18n](https://vimeo.com/352687255/d5140e06cd)
##[Implement I18n into your
codebase](https://vimeo.com/352687255/d5140e06cd)
1. Add basic configuration to your `./app/controllers/application_controller.rb`
    ![application controler
implementation](https://github.com/Khaleesicodes/github_students_package/blob/master/assets/carbon.png)

2. Set the languages in your `./config/initializers/locale.rb`
    ![setting
languages](https://github.com/Khaleesicodes/github_students_package/blob/master/assets/language.png)


# Connecting the project to phraseapp
## Install the Phrase CLI
  Run the following commands in your terminal
  1. `$brew tap phrase/brewed`
  2. `$brew install phraseapp`

## Phrase CLI Setup
  Run the following commands in your terminal
  1. `phraseapp init`
  2. Then you will be ask to provide an access token, which  you can
     create in the Phrase UI and copy paste it to your terminal
  3. Follow further instrudctions to setup a new project or choose an
     already existing project.
  4. When you get asked for the path just press enter, in our case the
     CLI already got the right path.
  5. All done?! Run your first `$phraseapp push`
  6. Play around in the Phrase UI and get all the changes with
     `$phraseapp pull`


> [**For futher information/ integrations also see our documentation
here**](https://help.phrase.com/en/?cjs=X2dhPUdBMS4yLjIwNzQ1NDA2NTguMTU1NDExNTIzNTsgaHVic3BvdHV0az1jZTM4MjM3MTFhODZjOWRjMDcyMmIzOGM1OWRkY2E2NDsgbWVzc2FnZXNVdGs9MTRkZTQwOGVkODg0NGIxM2JiNTg3ZmFlMmFmNGZhYjA7IF9mYnA9ZmIuMS4xNTU0MTkwNzU1OTkyLjQ0OTQ1MjY5NjsgX19hZHJvbGxfZnBjPWVjMWU5NjdmZTY1Y2FmNjI5ODk4ZmRhZDQzZDZmYzQwLXMyLTE1NTQxOTEwMzIxODE7IF9wYV92aWQ9MWVncDR0ai1uZnVnLW5tc29sbDsgX2hqaWQ9OTA3MWZlZTAtZTA1ZC00ZDRlLWI5MjgtNDgxMjE3ODg3ZWE1OyBfcGFfaWlkPW9mazdvMG80OyBfX2hzdGM9MjY2MzM3NTUyLmNlMzgyMzcxMWE4NmM5ZGMwNzIyYjM4YzU5ZGRjYTY0LjE1NTQxMTUyMzYwMDIuMTU2MzUyMzM3OTg3OS4xNTYzNTMxMDczNDAyLjIwMjsgX19hcl92ND1TVldYRDRGUVFCREtaQVRDUU9XNkZaJTNBMjAxOTA3MTclM0ExJTdDSElWTTZBQVFFRkJGRkdETERQR1FQSyUzQTIwMTkwNzAxJTNBMjQxJTdDV1BUQUVNQVJXSkZJVkZRSUtQTUNCRCUzQTIwMTkwNzAxJTNBMjQ0JTdDTElJRElSSkIzQkdVVkcyREc2TVNDNyUzQTIwMTkwNzAxJTNBMjQ0JTdDVklGSDJJWlVTVkdaRkk0VFBWTlAzVSUzQTIwMTkwNzE3JTNBMQ%3D%3D)




