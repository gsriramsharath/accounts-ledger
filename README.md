Goal: one repo that can compile/run REST + gRPC, generate types, and talk to Postgres.
Create repo accounts-ledger.


Add modules:


api/ → openapi.yaml, accounts.proto


service/ → Spring Boot app


service-grpc/ → gRPC server (can live inside service/ too)


migrations/ → Flyway SQL


tests/contract/ → Postman & grpcurl scripts


Add deps: Spring Web, Validation, Security, Data JPA, Flyway, Postgres; grpc, protobuf plugins; Testcontainers (Postgres).


Make sure ./gradlew build (or Maven) compiles both OpenAPI DTOs (if using generator) and protobuf stubs.
