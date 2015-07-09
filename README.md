# dokku-docker-auto-volumes

dokku-docker-auto-volumes is a plugin for [dokku][dokku] that automatically persist docker volumes declared in the Dockerfile.

## Requirements

* Dokku 0.3.17+ (for the `docker-options` plugin)

## Installation

```
git clone https://github.com/Flink/dokku-docker-auto-volumes /var/lib/dokku/plugins/docker-auto-volumes
dokku plugins-install
```

## Info

This plugin adds a `/etc/sudoers.d/dokku-docker-cp` file to allow ownership preservation when copying files from container to the host (using `docker cp`).

It will persist volumes into `$DOKKU_ROOT/$APP/.volumes`.

## License

This plugin is released under the MIT license. See the file [LICENSE](LICENSE).

[dokku]: https://github.com/progrium/dokku
