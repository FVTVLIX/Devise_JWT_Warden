# Devise_JWT_Warden

## Devise with a Rails API

### Objectives

- Build a easy to use full featured option to handle User Auth with a Rails API

`$ rails new devise_auth_app --api`

Once every thing is installed move into the `cd devise_auth_app` directory

lets install the required gems

```Ruby
gem 'devise'
gem 'jwt'

# we also need to uncomment
gem 'rack-cors'
```

and now run`$ bundle install`

---

Now that we have the required gems in our app, lets run the devise installer

`$ rails g devise:install`

when running this you will get this output in the console, don't worry about any of this now

```
===============================================================================

Some setup you must do manually if you haven't yet:

  1. Ensure you have defined default url options in your environments files. Here
     is an example of default_url_options appropriate for a development environment
     in config/environments/development.rb:

       config.action_mailer.default_url_options = { host: 'localhost', port: 3000 }

     In production, :host should be set to the actual host of your application.

  2. Ensure you have defined root_url to *something* in your config/routes.rb.
     For example:

       root to: "home#index"

  3. Ensure you have flash messages in app/views/layouts/application.html.erb.
     For example:

       <p class="notice"><%= notice %></p>
       <p class="alert"><%= alert %></p>

  4. You can copy Devise views (for customization) to your app by running:

       rails g devise:views

===============================================================================
```
