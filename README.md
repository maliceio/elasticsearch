![es-logo](https://raw.githubusercontent.com/maliceio/elasticsearch/master/es-logo.png)

# malice-elasticsearch

[![CircleCI](https://circleci.com/gh/maliceio/elasticsearch.png?style=shield)](https://circleci.com/gh/maliceio/elasticsearch) [![License](http://img.shields.io/:license-mit-blue.svg)](http://doge.mit-license.org) [![Docker Stars](https://img.shields.io/docker/stars/malice/elasticsearch.svg)](https://hub.docker.com/r/malice/elasticsearch/) [![Docker Pulls](https://img.shields.io/docker/pulls/malice/elasticsearch.svg)](https://hub.docker.com/r/malice/elasticsearch/) [![Docker Image](https://img.shields.io/badge/docker%20image-127MB-blue.svg)](https://hub.docker.com/r/malice/elasticsearch/)

Malice's Custom [Elasticsearch](https://www.elastic.co/products/elasticsearch) Docker Image

**Table of Contents**

- [Dependencies](#dependencies)
- [Image Tags](#image-tags)
- [Getting Started](#getting-started)
- [Documentation](#documentation)
- [Issues](#issues)
- [Credits](#credits)
- [CHANGELOG](#changelog)
- [Contributing](#contributing)
- [License](#license)

### Dependencies

- [alpine:3.8](https://index.docker.io/_/gliderlabs/alpine/)

### Image Tags

```bash
REPOSITORY               TAG                 SIZE
malice/elasticsearch   latest              127MB
malice/elasticsearch   6.4                 127MB
malice/elasticsearch   6.3                 122MB
malice/elasticsearch   6.0                 117MB
malice/elasticsearch   5.6                 124MB
malice/elasticsearch   5.5                 123MB
```

### Getting Started

```bash
$ docker run -d --name elastic -p 9200:9200 malice/elasticsearch
```

### Documentation

### Known Issues :warning:

I have noticed when running the new **5.0+** version on a linux host you need to increase the memory map areas with the following command

```bash
sudo sysctl -w vm.max_map_count=262144
```

### Issues

Find a bug? Want more features? Find something missing in the documentation? Let me know! Please don't hesitate to [file an issue](https://github.com/maliceio/elasticsearch/issues/new)

### Credits

Heavily (if not entirely) influenced by https://github.com/docker-library/elasticsearch
Production docs from https://stefanprodan.com/2016/elasticsearch-cluster-with-docker/

### CHANGELOG

See [`CHANGELOG.md`](https://github.com/maliceio/elasticsearch/blob/master/CHANGELOG.md)

### Contributing

[See all contributors on GitHub](https://github.com/maliceio/elasticsearch/graphs/contributors).

Please update the [CHANGELOG.md](https://github.com/maliceio/elasticsearch/blob/master/CHANGELOG.md) and submit a [Pull Request on GitHub](https://help.github.com/articles/using-pull-requests/).

### License

MIT Copyright (c) 2016-2018 **blacktop**
