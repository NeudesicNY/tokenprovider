# Token Provider

TBD

## Running locally

1. Install and start the Cosmos DB emulator.
2. Open solution in VS and make sure the Environment variables are set in the `TokenProvider` project
2. Build and start the `TokenProvider` project
3. Send a GET request to `http://localhost:7071/api/cosmos/token` with a `token` header containing a JWT token which has a `upn` claim
4. Response should contain an array of resource tokens 

## Roles

There is only 1 role supported today named "Default".

## Config

- `TOKEN_PROVIDER_COSMOS_ENDPOINT`: URL of the Cosmos DB resource (aka https://localhost:8081)
- `TOKEN_PROVIDER_COSMOS_MASTERKEY`: Master Key of the Cosmos DB resource
- `TOKEN_PROVIDER_COSMOS_DEFAULT`: Permission string for the "Default" role
- `TOKEN_PROVIDER_COSMOS_DEFAULT_KEYS`: Keys for environment variables that contain permission strings for the "Default" role

## License

[MIT](LICENSE)