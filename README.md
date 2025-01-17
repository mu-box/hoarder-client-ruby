# hoarder

A Ruby client for interacting with the [hoarder](https://github.com/mu-box/hoarder) service.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'hoarder'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install hoarder

## Usage

#### Client

Instantiate a client, providing the IP of the host and the security token:
```ruby

client = Hoarder::Client.new('127.0.0.1', 'secret')

```

#### Blobs

List all blobs
```ruby
client.blobs
```

Fetch metadata about a specific blob
```ruby
client.blob(id)
```

Remove a blob:
```ruby
client.remove_blob(id)
```

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake spec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/mu-box/hoarder.


## License

This project is released under [The MIT License](http://opensource.org/licenses/MIT).
