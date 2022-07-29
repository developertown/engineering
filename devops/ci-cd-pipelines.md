# CI/CD Pipeline Building

Let's start with what makes for a good application pipeline.  There are many resources out there for diving into the specifics as to the why's but for this section we're going to focus specifically on the what.

Fundamental pipeline characteristics:

* Static analysis is performed on the code
  * Identification of problamtic patterns 
  * Code format consistency
* Verify selected open source or 3rd party tools use compatible license
* Security scans
  * Check deployment artifact for known CVEs
  * Check dependencies for known CVEs
* Compiles all code
* Runs all unit, integration, and acceptance tests
* Builds a deployment artifact such as an OCI compliant image like docker

* Automatically deploys to minimally a dev environment, ideally linearly into stage
* Executes a smoke test to confirm the application is working
* Automatic rollbacks when the smoke test fails
* Application health checks to confirm the container is ready to receive traffic
* The app is following 12 factor
* Optionally gated deployments to production