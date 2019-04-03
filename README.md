# Docker image of *dex*

![dex](https://github.com/dexidp/dex/raw/master/Documentation/logos/dex-horizontal-color.png)

Dex is an identity service that uses [OpenID Connect][openid-connect] to drive authentication for other apps.

Dex acts as a portal to other identity providers through ["connectors."](#connectors) This lets dex defer authentication to LDAP servers, SAML providers, or established identity providers like GitHub, Google, and Active Directory. Clients write their authentication logic once to talk to dex, then dex handles the protocols for a given backend.

Read more about dex [here](https://github.com/dexidp/dex#dex---a-federated-openid-connect-provider)

## Simple usage

```bash
$ docker run --name dex \ 
  -p 5556:5556 \
  -v "${PWD}/dex-config.yaml:/config.yaml" \
  -v "${PWD}/web:/web" \
  navrocky/dex serve /config.yaml
```

Where:
`-p 5556:5556` where HTTP endpoint is

`-v "${PWD}/dex-config.yaml:/config.yaml"` - your dex configuration file. See at example [config](https://github.com/dexidp/dex/blob/v2.15.0/examples/config-dev.yaml)

`-v "${PWD}/web:/web"` - optional directory with web static resources, forms and themes.


## Docker compose

```yaml
TODO
```
