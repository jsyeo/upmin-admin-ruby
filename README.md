# No Longer Actively Maintained

Upmin Admin is no longer under active development. We recommend that you check out [Administrate](https://github.com/thoughtbot/administrate) if you are in need of an admin framework. It is created by the people at [thoughtbot](https://thoughtbot.com/).

# Upmin Admin
[![Gem Version](https://badge.fury.io/rb/upmin-admin.svg)](http://badge.fury.io/rb/upmin-admin)

Upmin Admin is a framework for creating powerful Ruby on Rails admin backends with minimal effort.
Upmin currently supports Rails 3.2, 4.0, 4.1 & 4.2.


## Demo Applications

There is a demo application you can test out here: [store_demo](https://github.com/upmin/store_demo).

If you do choose to use the [store_demo](https://github.com/upmin/store_demo), please follow the directions in the [README](https://github.com/upmin/store_demo/blob/master/README.md) to ensure you have seed data to work with.

You can also generate a starter application using [Rails Composer](http://www.railscomposer.com/) that sets up Devise, role-based authorization, and upmin-admin. See [Upmin Admin Interface in Rails Composer](http://blog.railsapps.org/post/97584175990/upmin-admin-interface-in-rails-composer).


## Installation

Installing `upmin-admin` is incredibly easy. Simple add the gem to your `Gemfile`:

```ruby
gem 'upmin-admin'
```

Then run the generator:

```ruby
rails g upmin:install
```

This mounts the engine in your `routes.rb` file:

```ruby
mount Upmin::Engine => '/admin'
```

And adds a configuration file at `config/initializers/upmin.rb`

If you already have routes pointing to `/admin` you can use any path you want, for example you could use the following instead:

```ruby
mount Upmin::Engine => '/ice-ice-baby'
```

And you would access your admin page at `localhost:3000/ice-ice-baby` or `example.com/ice-ice-baby`.

If you prefer not to use the generator, simply add the route, and optionally the config file as documented in the wiki.

## Documentation

For further documentation, please visit our [Wiki](https://github.com/upmin/upmin-admin-ruby/wiki). The docs there are far from complete, but we are actively updating them. If you have any trouble or can't find the documentation to do something please [create an issue](https://github.com/upmin/upmin-admin-ruby/issues) and contribute to the docs where you can.


## Going Forward

Upmin Admin is new. It has been live for less than a few months, so there are going to be things missing. If you want to make it better, get involved and [create issues](https://github.com/upmin/upmin-admin-ruby/issues) when you find bugs or want new features, and [contribute](https://github.com/upmin/upmin-admin-ruby/blob/master/CONTRIBUTING.md) with pull requests.

The major features that are being worked on now are:

1. Mongoid support
2. Fixing bugs as we find them
3. Adding widgets
4. Implementing the dashboard


## Support & Feedback

We are always looking for feedback and suggestions. We prefer that you create a GitHub issue, but you can use any of the following to contact us:

Email - [support+admin@upmin.com](support+admin@upmin.com)

Twitter - [@UpminSupport](https://twitter.com/upminsupport)

GitHub - [Create an Issue](https://github.com/upmin/upmin-admin-ruby/issues)

Please note that this is an open source project, and we can't always respond immediately, but we do try to respond to all inquiries within 24 hours and are usually much faster to respond.
