# Demo connector

Based on
- https://github.com/jhalasinski/connector-local.git
- https://github.com/eclipse-edc/Samples/tree/main/transfer

## Changes
- Project updated to EDC v. 0.7.0
- Jupyter notebook updated accordingly to interact with EDC v. 0.7.0
- Replaced postgres-flyway Extension (incompatible with EDC starting from EDC v. 0.5.0) with migrations from TractusX
- Updated data-dashboard-local Extension, updating think-it-labs/edc-connector-client package to v. 0.5.0 & adding manual changes to the project

## Build
1. `cd ./src`
2. `./gradlew launcher:build`

## How to run
1. `cd ./compose`
2. `docker compose -f base.yaml up --build`

## Next steps
- Same as declared in https://github.com/jhalasinski/connector-local/tree/main/src
