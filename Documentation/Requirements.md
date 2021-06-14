# Zowe APIML Metrics Service Requirements

## Business Requirements
* Maintain security of Zowe APIML and applications being monitored
* Allow administrators to see HTTP metrics of REST API endpoints of each service onboarded to the APIML
* Allow administrators to see system metrics of each service onboarded to the APIML
* Provide guidance to users of the new Metrics Service and how to interact with it
* Provide feedback mechanisms for users to provide feedback on the new Metrics Service

## Functional Requirements
* Registers to the Discovery Service
* Use Gateway to route user to Metrics Service UI
* Use Gateway authentication and support Gateway SSO
* Metrics are streamed to provide real-time metrics
* Metrics solutions are able to run on and off Z
* Able to run with multiple instances for a highly available configuration
* Metrics Service starts via a launch component group from Zowe `instance.env`

## Non-Functional Requirements
* Implemented such that static configuration can be used to control most aspects of the behaviour
* Implemented such that any HTTP and system metrics collection service can be plugged into the Metrics Service