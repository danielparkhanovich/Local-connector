# Build
`./gradlew clean build`

# How to run
`docker compose up --build`

# Info
Provider in order to run need: 
- `Dedc.keystore` (cert.pfx), 
- `Dedc.keystore.password`, 
- `Dedc.vault` (...-vault.properties), 
- `Dedc.fs.config` (...configuration.properties)
- `jar` -> .../connector.jar
Consumer need (same):
- `Dedc.keystore`
- `Dedc.keystore.password`
- `Dedc.vault`
- `Dedc.fs.config`
- `jar`

# Links:
Repo with deployed v.0.3.1 connectors: https://gitlab.pcss.pl/dpi-pipelines/edc-connector/edc-connector
Jan local deployment v.0.3.1: https://github.com/jhalasinski/connector-local
EDC repo: https://github.com/eclipse-edc/Connector