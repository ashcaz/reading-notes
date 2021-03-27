# API Deployment

**LINKS**

- [Django Settings Best Practices](https://djangostars.com/blog/configuring-django-settings-best-practices/)
- [SSH Tutorial](https://www.hostinger.com/tutorials/ssh-tutorial-how-does-ssh-work)
- [White Noise](http://whitenoise.evans.io/en/stable/)
- [IaaS](https://en.wikipedia.org/wiki/Infrastructure_as_a_service)
- [PaaS](hhttps://en.wikipedia.org/wiki/Platform_as_a_service)
- [CORS](https://en.m.wikipedia.org/wiki/Cross-origin_resource_sharing)

## Django Settings Best Practices

### Different Enviornments

Usually, you have several environments: local, dev, ci, qa, staging, production, etc. Each environment can have its own specific settings (for example: DEBUG = True, more verbose logging, additional apps, some mocked data, etc). You need an approach that allows you to keep all these Django setting configurations.

### Sensitive data

You have SECRET_KEY in each Django project. On top of this there can be DB passwords and tokens for third-party APIs like Amazon or Twitter. This data cannot be stored in VCS.

## How Does SSH Work

SSH, or Secure Shell, is a remote administration protocol that allows users to control and modify their remote servers over the Internet. The service was created as a secure replacement for the unencrypted Telnet and uses cryptographic techniques to ensure that all communication to and from the remote server happens in an encrypted manner. It provides a mechanism for authenticating a remote user, transferring inputs from the client to the host, and relaying the output back to the client.

[Back to Homepage](https://ashcaz.github.io/reading-notes)
