# DigitalOcean autodiscovery plugin for Automatron

This plugin provides autodiscovery of DigitalOcean droplet servers.

## Installation

To install this plugin simply copy the `digitalocean` directory into Automatron's `plugins/discovery/` directory.

```shell
$ cp -r digitalocean/ plugins/discovery/
```

Install requirements with `pip`.

```shell
$ pip install -r requirements.txt
```

## Configuration

This plugin does require some configuration in Automatron's master configuration file `config.yml`.

```yaml
discovery:
  plugins:
    digitalocean:
      url: http://example.com
      api_key: example
      interval: 60
```

The `digitalocean` plugin requires two configuration items.

* `url` - This is the URL of Digital Ocean's API
* `api_key` - This is the Digital Ocean API key
* `interval` - This is the frequency to query Digital Ocean's API

