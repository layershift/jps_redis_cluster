PHP.ini settings:
```
session.save_handler = rediscluster
session.save_path = "seed[]=${nodes.redis_nodes[0].address}:${settings.fm}&seed[]=${nodes.redis_nodes[1].address}:${settings.sm}&seed[]=${nodes.redis_nodes[2].address}:${settings.tm}&seed[]=${nodes.redis_nodes[3].address}:${settings.fs}&seed[]=${nodes.redis_nodes[4].address}:${settings.ss}&seed[]=${nodes.redis_nodes[5].address}:${settings.ts}&timeout=2&read_timeout=2&failover=error&persistent=1&auth=${globals.pass}&stream[verify_peer]=0"
```

[P3X Redis UI](https://developer:${globals.pass}@node${nodes.redis_nodes[0].id}-${env.domain}/connect/)
Access details:

User: developer\
Password: ${globals.pass}
