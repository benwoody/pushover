# Pushover

This gem provides a CLI and an API interface to http://pushover.net

Currently it's a work in process and I haven't built out the CLI yet, that will happen shortly.

## Installation

To install:

    $ gem install pushover

To use inside of an application, add this to the your gemfile:

		$ gem 'pushover'

and run bundle to make it available:

		$ Bundle

## Usage

Progmatic usage:

```ruby
require 'pushover'

Pushover.notification('your_token', 'app_token', 'message', 'title')
```

Title is currently optional, it doesn't do more then this yet.

CLI usage:

		$ pushover -a apitoken -t token -m 'message goes in here' -t 'title is optional.'


## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Added some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request
