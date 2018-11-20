
## Testing Configuration

A testing environment of this test bench is consisted of Docker technology and the configuration is as follows;

```
+---------+
| Your    +--(Shared source code under ../src)
| Desktop +--(Shared resources under ./)
+----+----+
     |   docker's virtual network
-----+--------------+-------------+----------
     |              |             |
+----+----+    +----+----+   +----+----+
| Target  |    | MongoDB |   | Tester  |
| Asterisk|    |         |   |         |
+---------+    +---------+   +---------+
asterisk       ast_mongo     tester
```

### How to test

- see [./test](test)

## Requirements

- [Docker](https://www.docker.com)
  - e.g. [Docker Community Edition for Mac](https://store.docker.com/editions/community/docker-ce-desktop-mac), Version 2.0.0.0-mac78
