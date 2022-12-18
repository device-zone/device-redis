# device-redis
Provides a redis server appliance.

This appliance does the following:

- All parameters passed to the device commands are syntax checked and canonicalised, with bash completion.
- Automatically configures redis's configuration files before startup.
- Binds securely to the unix domain socket /run/redis/redis.sock.
- Autostarts when called for by other services.
- Zero Trust configuration.

This package does unix domain sockets at this time. In future, a device-redis-tls package will add TLS support.

## before

- Deploy the device-redis package.

```
[root@server ~]# dnf install device-redis
```

