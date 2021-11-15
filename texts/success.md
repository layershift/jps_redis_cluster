In order to use the cluster please connect to the following nodes:

${globals.nodes.redis_nodes[0].address:${settings.fm}\
${globals.nodes.redis_nodes[1].address:${settings.sm}\
${globals.nodes.redis_nodes[2].address:${settings.tm}\
${globals.nodes.redis_nodes[3].address:${settings.fs}\
${globals.nodes.redis_nodes[4].address:${settings.ss}\
${globals.nodes.redis_nodes[5].address:${settings.ts}


Password: ${globals.pass}

[P3X Redis UI](https://developer:${globals.pass}@node${globals.nodes.redis_nodes[0].id}-${globals.env.domain}/connect/)
Access details:

User: developer\
Password: ${globals.pass}

Check the "Redis Cluster Tools" add-on for more actions