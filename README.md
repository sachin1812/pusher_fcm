# pusher_fcm
A simple gem for sending push notifications in Android and iOS devices

Installation
```ruby
$ gem install pusher_fcm
```
or in your Gemfile just include it:
```ruby
gem 'pusher_fcm'
```
# Requirements

One of the following, tested Ruby versions:
```ruby
2.0.0
2.1.9
2.2.5
2.3.1
```
# Usage

Example sending notifications:
```ruby
require 'pusher_fcm'

fcm = PUSHER_FCM.new("API-KEY")

device_token= ["xxxxxxxx", "xxxxxxx"] # an array of one or more client device tokens

fcm.title="My Title"

fcm.body ="My Body"

response = fcm.send(device_token)
```

# Thanks 
