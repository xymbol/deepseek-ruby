# Deepseek

A Ruby client for accessing the DeepSeek API.

## Installation

Install the gem and add to the application's Gemfile by executing:

```bash
bundle add deepseek
```

If bundler is not being used to manage dependencies, install the gem by
executing:

```bash
gem install deepseek
```

## Usage

```ruby
client = Deepseek::Client.new("your-api-key")

response = client.chat_completions(
  model: "deepseek-chat",
  messages: [{role: "user", content: "Hello, world!"}]
)
```

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run
`rake test` to run the tests. You can also run `bin/console` for an interactive
prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To
release a new version, update the version number in `version.rb`, and then run
`bundle exec rake release`, which will create a git tag for the version, push
git commits and the created tag, and push the `.gem` file to
[rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at
https://github.com/xymbol/deepseek-ruby.

## License

The gem is available as open source under the terms of the [MIT
License](https://opensource.org/licenses/MIT).
