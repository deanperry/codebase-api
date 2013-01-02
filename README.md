# CodebaseApi

A gem to interact with the [Codebase](http://www.codebasehq.com) API.

## Installation

Add this line to your application's Gemfile:

    gem 'codebase_api'

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install codebase_api

## Usage

The Codebase API requires authentication using your account name & username along with your API Key.

In a Rails app, create a file called `config/initializers/codebase.rb` and fill it with this info (changing it for your account, etc)

```ruby
CodebaseApi.account_user = "account/user"
CodebaseApi.api_key = "apikey"
```

## Commands

The CodebaseApi gem is built to access all the Codebase API functions.

#### Displays a list of all projects on your Codebase account
```ruby
CodebaseApi::Project.all
```

#### Shows a specific project
```ruby
CodebaseApi::Project.view("my-cool-project")
```

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request