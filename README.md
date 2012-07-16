# CatarseDineromail

Dineromail integration with Catarse crowdfunding platform

## Installation

Add this line to your application's Gemfile:

    gem 'catarse_dinero'

And then execute:

    $ bundle

## Usage

Configure the routes for your Catarse application. Add the following lines in the routes file (config/routes.rb)
    
    mount CatarseDineromail::Engine => "/", :as => "catarse_dineromail"

Create required configurations into Catarse database:
    
    dineromail_merchant

    dineromail_ipn_password

    dineromail_country_id

## Development environment setup

Clone the repository

    $ git clone git://github.com/josemarluedke/catarse_dineromail.git

Add the catarse code into test/dummy

    $ git submodule add git://github.com/danielweinmann/catarse.git test/dummy

Copy the Catarse's gem into Gemfile

    $ cat test/dummy/Gemfile >> Gemfile

And then execute:

    $ bundle

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request


This project rocks and uses MIT-LICENSE.