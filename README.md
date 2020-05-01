<p align="center">
<img src="https://raw.githubusercontent.com/OneTrackingFramework/documentation/master/otf_logo.png" width=300/>
</p>

# One Tracking Framework

The One Tracking Framework (OTF) is supposed to offer generic and reusable backend implementations to speed up application development. The OTF got founded as a response to the COVID-19 crisis.

Services / backend components are intended to be implemented as micro services to enable high scalability by design.

In order to enable independent development to focus on the same goal, we introduced a macro architecture, each implementation must be consistent with.

# Macro Architecture

- Microservices
- APIs implement REST endpoints
- Internal communication between services is based on event store (event driven design) or direct HTTP communication (with the risk of data loss)
- Services must be stateless in order to run as multiple instances
- Use GitHub for Repositories (Preferably https://github.com/OneTrackingFramework)
- Preferably use Google Code Style if possible (https://github.com/google/styleguide)
- Preferably use a technology stack, that is well-known and supported by corporations as those are more likely to be accepted
- The license of each service should be the MIT license preferably to offer as less limitation as possible

# Current well-advanced services

| Service | Purpose / Description |
|---|---|
| survey-service | Generic survey implementation to define survey question and answer meta data, receiving survey responses and generating analytics on top of the collected data |
| push-notification-service | Sending push notifications based on Firebase Cloud Messaging |
| tcn-service | An implementation of the TCN backend |
