# Environments

DeveloperTown projects will typcially utitlize at least **two** deployed environments. A typical setup will include a `Test` environment used internally by developers to verify working code as it is integrated into the larger application. DeveloperTown projects _may_ promote code changes directly from the `Test` environment to a `Production` environment in the simpliest of configurations. Depending on project/client need there may be additional environments such as `Staging`, `UAT`, `Perf`, etc that sit between the `Test` environment and the `Production` environment to facilitate specific testing needs.

## Managing Configuration for multiple environments
