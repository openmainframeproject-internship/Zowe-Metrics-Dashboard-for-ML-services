**Student's Name:** Saurabh Raj

**Mentor:** Carson Cook

**Project:** Zowe APIML Metrics Service

**Project Description:**
Create a microservice that will collect and display transport and system metrics for API Mediation Layer services.

**Problem Definition:**
System administrators using Zowe and the API Mediation Layer want to understand the overall health, security, and performance of the Mediation Layer and its onboarded services. Currently, there is no integrated way to view metrics that give insight in these areas.

**Deliverables**

* A new "Metrics Service" microservice in the Zowe APIML
* HTTP metrics for each APIML service are collected by Netflix Hystrix and aggregated by Netflix Turbine
* HTTP metrics for each APIML service are displayed with a React-embedded Hystrix/Turbine dashboard
* Display system metrics collected by a third party service in a third party UI dashboard
* Integrate the Metrics Service and all of its endpoints into the APIML and its features, such as authentication and routing
* Provide a UI tour and tutorial for new users of the Metrics Service

**Coding Plan**

| Week | Tasks | Goals |
|------|-------|-------|
| Week 3 | [#867](https://github.com/zowe/api-layer/issues/867) | Enable Hystrix metrics stream for a test APIML service. |
| Week 4 | [#868](https://github.com/zowe/api-layer/issues/868) | Enable the Hystrix dashboard and embed it in the React UI. |
| Week 5 | [#869](https://github.com/zowe/api-layer/issues/869) | Enable Turbine to aggregate Hystrix across multiple service instances. |
| Week 6 | [#870](https://github.com/zowe/api-layer/issues/870) | Create configuration properties that allow the user to enable/disable Hystrix and Turbine for certain service endpoints. |
| Week 7 | Use case diagrams for HTTP metrics. [#1099](https://github.com/zowe/api-layer/issues/1099) | Use case diagrams for user actions with HTTP metrics. Select UI dashboard to display system metrics. |
| Week 8 & 9 | [#1101](https://github.com/zowe/api-layer/issues/1101) | Select a system metrics collection service and connect it to the UI dashboard selected in #1099. |
| Week 10 | [#1045](https://github.com/zowe/api-layer/issues/1045)] | Write user documentation and create a UI tour through the Metrics Service. |
| Week 11 | [#1114](https://github.com/zowe/api-layer/issues/1114). [#1100] | Write Metrics Service smoke tests for the Zowe build pipeline. Add feedback mechanism links and descriptions to the Metrics Service UI. |
| week 12 | Buffer or identified stretch goals | - |
