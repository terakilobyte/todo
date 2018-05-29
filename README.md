# README

This project contains two git submodules, client and server, which comprise
this todo service.

## Building

There are 3 docker-compose files

### .unit

This is the compose file for developing and testing each individual service in
isolation.

The end to end tests in the client service will fail in this mode.

### .test

This is the compose file for developing and testing end to end.

### .prod

This is the compose file for deplying the service. A build is made of the client
and then served with nginx. Logging is removed from the server.
