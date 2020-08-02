# Launchpad-Schema
Contains the global schema definition for message exchange used by the Launchpad Project

## Schema Definitions

|S/No|Filename|Description                                                    |
|----|--------|---------------------------------------------------------------|
|1|system.proto|Message definition for all system related messages e.g. Logs, Metrics|
|2|app.proto|Message definition for all app related messages e.g. App Added, Removed, Updated|

## Usage

### Go Lang

1. Install Protobuf Compiler. [See Compiling Protocol Buffers](https://developers.google.com/protocol-buffers/docs/gotutorial#compiling-your-protocol-buffers)

2. Generating Protobuf Stubs
    
    ```bash
    $ protoc -I=./launchpad-schema -I=./launchpad-schema/include --go_out=./launchpad-agent launchpad-schema/metrics.proto
    ```


