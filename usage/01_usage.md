!SLIDE code
## La config ##

    @@@ YAML
    server: www.myapp.com
    email: "no-reply@myapp.com"
    facebook_token: "AAABBBCCC"

!SLIDE code
## Mais aussi ##

    @@@ YAML
    lang: <%= ENV['LANG'] %>
    redis:
      server: localhost
      port: 6379

!SLIDE code
## Dans l'application ##

    @@@ ruby
    Settings.server #=> "www.myapp.com"
    Settings.redis.server #=> "localhost"
    Settings[:redis][:port] #=> 6379
