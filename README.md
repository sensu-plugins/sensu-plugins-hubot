## Sensu-Plugins-hubot

[![Build Status](https://travis-ci.org/sensu-plugins/sensu-plugins-hubot.svg?branch=master)](https://travis-ci.org/sensu-plugins/sensu-plugins-hubot)
[![Gem Version](https://badge.fury.io/rb/sensu-plugins-hubot.svg)](http://badge.fury.io/rb/sensu-plugins-hubot)
[![Code Climate](https://codeclimate.com/github/sensu-plugins/sensu-plugins-hubot/badges/gpa.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-hubot)
[![Test Coverage](https://codeclimate.com/github/sensu-plugins/sensu-plugins-hubot/badges/coverage.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-hubot)
[![Dependency Status](https://gemnasium.com/sensu-plugins/sensu-plugins-hubot.svg)](https://gemnasium.com/sensu-plugins/sensu-plugins-hubot)

## Functionality

## Files
 * bin/handler-hubot

## Usage

```
{
  "hubot": {
    "server": "hubot.domain.tld",
    "port": 8080,
    "channel": "#irc-room"
  }
}
```
## Installation

Add the public key (if you haven’t already) as a trusted certificate

```
gem cert --add <(curl -Ls https://raw.githubusercontent.com/sensu-plugins/sensu-plugins.github.io/master/certs/sensu-plugins.pem)
gem install sensu-plugins-hubot -P MediumSecurity
```

You can also download the key from /certs/ within each repository.

#### Rubygems

`gem install sensu-plugins-hubot`

#### Bundler

Add *sensu-plugins-disk-checks* to your Gemfile and run `bundle install` or `bundle update`

#### Chef

Using the Sensu **sensu_gem** LWRP
```
sensu_gem 'sensu-plugins-hubot' do
  options('--prerelease')
  version '0.0.1'
end
```

Using the Chef **gem_package** resource
```
gem_package 'sensu-plugins-hubot' do
  options('--prerelease')
  version '0.0.1'
end
```

## Notes
