# Demo connector

Based on
- https://github.com/jhalasinski/connector-local.git
- https://github.com/eclipse-edc/Samples/tree/main/transfer

## Changes
- Project updated to EDC v. 0.7.0
- Jupyter notebook updated accordingly to interact with EDC v. 0.7.0
- Removed postgres-flyway Extension (incompatible with EDC starting from EDC v. 0.5.0)
- Removed data-dashboard-local Extension (incompatible with EDC v.0.7.0 starting from EDC v. 0.?.?)

## Build
1. `cd ./src`
2. `./gradlew clean build`

## How to run
1. `cd ./compose`
2. `docker compose up --build`

## Next steps
- Add extension for dashboard (not investigated yet)
- Same as declared in https://github.com/jhalasinski/connector-local/tree/main/src
