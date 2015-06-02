# mruby-mutex   [![Build Status](https://travis-ci.org/matsumoto-r/mruby-mutex.png?branch=master)](https://travis-ci.org/matsumoto-r/mruby-mutex)
Mutex class
## install by mrbgems
- add conf.gem line to `build_config.rb`

```ruby
MRuby::Build.new do |conf|

    # ... (snip) ...

    conf.gem :github => 'matsumoto-r/mruby-mutex'
end
```
## example
```ruby
p Mutex.hi
#=> "hi!!"
t = Mutex.new "hello"
p t.hello
#=> "hello"
p t.bye
#=> "hello bye"
```

## License
under the MIT License:
- see LICENSE file
