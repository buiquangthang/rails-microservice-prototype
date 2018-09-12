# Rails Microservice API Gateway prototype
This is mixing up of some API designs for microservice using Rails

## Setting up

### API Gateway
```bash
cd Rails-API-Auth
# edit config/database.yml
rake db:create db:migrate db:seed
rails s -p 5000
```

### Post service
```bash
cd post_service
rake db:create db:migrate db:seed
rails s -p 5001
```

References:

Rails token-based authentication blueprint
https://github.com/jameskropp/Rails-API-Auth

Template for a basic authorization API using Ruby on Rails.
Tutorial Link - https://medium.com/@jkropp/building-a-simple-token-based-authorization-api-with-rails-a5c181b83e02

Ruby on Rails API Gateway
API gateway serves as single point of entry to microservices and for all client types. The idea is to provide a single entry point for all the fine-grained APIs of the individual services. This is a simple api routing app.
https://github.com/rzkmr/gateway

JWT-Ruby https://github.com/jwt/ruby-jwt
Knock gem https://github.com/nsarno/knock
