# Docker image of *dex*

![dex](https://github.com/dexidp/dex/raw/master/Documentation/logos/dex-horizontal-color.png)

Dex is an identity service that uses [OpenID Connect][openid-connect] to drive authentication for other apps.

Dex acts as a portal to other identity providers through ["connectors."](#connectors) This lets dex defer authentication to LDAP servers, SAML providers, or established identity providers like GitHub, Google, and Active Directory. Clients write their authentication logic once to talk to dex, then dex handles the protocols for a given backend.

Read more about dex [here](https://github.com/dexidp/dex#dex---a-federated-openid-connect-provider)

## Simple usage

```bash
$ docker run 
```

## Docker compose

```yaml
```
