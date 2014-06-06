Ansible elasticsearch
=====================

Installs latest version of elasticsearch and it's plugins

Requirements
------------

No

Role Variables
--------------

```
elasticsearch:
  deb: https://download.elasticsearch.org/elasticsearch/elasticsearch/elasticsearch-1.2.1.deb
  deb_sha256: 83e2bd6849847b9f0f922d469b74d43c00a428d100b18b4e71077f29864188fb
  plugins:
    - name: mobz/elasticsearch-head
      creates: head
    - name: karmi/elasticsearch-paramedic
      creates: paramedic
    - name: lukas-vlcek/bigdesk
      creates: bigdesk
  config: {}
```

Dependencies
------------

- `kunik.java`

License
-------

BSD
