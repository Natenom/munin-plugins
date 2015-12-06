# Munin-Plugins
Several plugins for [MUNIN](http://munin-monitoring.org/).

## minecraft_
Description: Shows user count and RAM usage.

[Project page (German)](https://wiki.natenom.de/minecraft/munin-plugin)

### Installation
As the script needs root rights to work correctly, you must add following
two lines to /etc/munin/plugin-conf.d/munin-node on Debian:
  [minecraft_*]
  user root

If your server is running on the default port, do as root (or with sudo):
```
  cd /etc/munin/plugins
  ln -s /path/to/minecraft_ minecraft_25565
```

## murmur-munin.py
A MUNIN plugin to query a Mumble-Server (Murmur).

Available data:
* users (all)
* users (muted)
* users (registered)
* users (not registered)
* ban count
* channel count/10
* server uptime in days

Documentation (English): https://wiki.natenom.com/w/Munin_plugin_for_a_Murmur_%28Mumble-Server%29
Documentation (German): https://wiki.natenom.de/mumble/tools/munin

### Features
* Support to set [messagesizemax](https://wiki.natenom.de/mumble/benutzerhandbuch/murmur/messagesizemax) value.

