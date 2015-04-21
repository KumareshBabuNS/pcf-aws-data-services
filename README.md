Service Brokers
===============

A Spring Boot app that makes AWS data services available via a service broker using the [Service Broker API for CloudFoundry](http://docs.cloudfoundry.org/services/api.html)

This app can be deployed within CloudFoundry as well.

The manifest.yml files for each app include the following constants:
* `SVC_AUTH_NAME`: this is the authentication name the `CloudController` will use to auth with the broker
* `SVC_AUTH_CODE`: this is the authentication code the `CloudController` will use to auth with the broker

When adding a service broker, you can use the following command:
`cf update-service-broker {service_name} {SVC_AUTH_NAME} {SVC_AUTH_CODE} {service_app_endpoint}`

