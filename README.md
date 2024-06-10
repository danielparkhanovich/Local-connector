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
- Add extension for persistence 
    - first option is to modify Sovity Extension: adjust extension and replace db migrations with migrations from https://github.com/eclipse-tractusx/tractusx-edc/tree/main/edc-extensions/migrations/control-plane-migration (not the best option due to the added difficulty of  maintaining the custom extension)
    - second option is to adopt TractusX extensions for persistence using setup 2: https://github.com/eclipse-tractusx/tractusx-edc/tree/main/docs (more preferable)
- Add extension for dashboard (not investigated yet)
- Same as declared in https://github.com/jhalasinski/connector-local/tree/main/src