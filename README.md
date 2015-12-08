# dokku-docker-auto-volumes

dokku-docker-auto-volumes is a plugin for [dokku][dokku] that automatically persist docker volumes declared in the Dockerfile.

## Requirements

* Dokku 0.3.17+ (for the `docker-options` plugin)

## Installation

```shell
# dokku 0.3.26
$ git clone https://github.com/Flink/dokku-docker-auto-volumes /var/lib/dokku/plugins/docker-auto-volumes
$ dokku plugins-install

# dokku 0.4+
$ dokku plugin:install https://github.com/Flink/dokku-docker-auto-volumes.git
```

## Info

This plugin will persist volumes into `/var/lib/dokku/volumes/$APP`.

## License

This plugin is released under the MIT license. See the file [LICENSE](LICENSE).

[dokku]: https://github.com/progrium/dokku
