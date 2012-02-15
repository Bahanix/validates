# Validates

## Summary

Email, Slug, Url simple format validators for Rails 3

## Installing

Add this to your `Gemfile`:

    gem "validates"

## Usage

    model User < ActiveRecord::Base
      validates :email, :email => true
      validates :site, :url => true, :allow_blank => true
      validates :inn, :inn => true   
    end

    model Page < ActiveRecord::Base
      validates :slug, :slug => true
    end


## Relise notes

0.0.2 - Fixed email validator. If email not presence, should be validate anyway.
0.0.3 - Add inn  validator. 

## Similar

* http://github.com/balexand/email_validator
* http://github.com/cesario/activevalidators
* https://rubygems.org/gems/date_validator
* and more...
