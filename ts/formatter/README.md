- `./compatible`: format adapter to cater backward compatibility 
- `./proto`: manipulating protobuf serialize/deserialize 
- `./fs`: relying on native library 'fs' 

## Configuration justification
### tsconfig.json
- compilerOptions
  - `moduleResolution`: let typescript use native node modules (not for commonjs)
  - `esModuleInterop`: true,
    - Resolve `ts-jest[config] (WARN) message TS151001`

## Dependency justification
- `google-protobuf`: used for message `Timestamp`, which is excluded from fabric-protos

 