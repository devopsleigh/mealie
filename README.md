# Mealie

## Description

Recipe managment and meal planning.

## Notes

- Uses unique container user
- Does not require additional privileges

## Configuration

1. Fill in the `.env` file as per the `compose.yml`

## Authentication

Mealie uses OIDC with Keycloak:
[Ref](https://docs.mealie.io/documentation/getting-started/authentication/oidc/)

### Keycloak setup

Create an OIDC client named `mealie`

Name | Value
---- | -----
Root URL | `https://mealie.yourDomain`
Redirect URIs | `/login?direct=1`<br>`/login`
Valid post logout redirect URIs | `/login?direct=1`<br>`/login`
Authentication flow | Enable: `Standard flow`<br>`Direct access grants`
<!-- 
## Logging

## Backup -->

## Links

- [Mealie docs](https://docs.mealie.io/documentation/getting-started/introduction/)
