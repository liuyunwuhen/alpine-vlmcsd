## Usage

Here are some example snippets to help you get started creating a container.

### docker-compose 

```bash
---
version: "2"
services:
  vlmcsd:
    image: liuyunwuhen/alpine-vlmcsd:arm64v8-v1113
    container_name: vlmcsd-v1113
    ports:
      - "1688:1688"
    restart: unless-stopped
```

### docker cli

```bash
docker run -d -p 1688:1688 --restart=unless-stopped liuyunwuhen/alpine-vlmcsd:arm64v8-v1113
```

