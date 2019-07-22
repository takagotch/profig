### profig
---
https://profig.readthedocs.io/en/default/

```py
cfg = profig.Config()
cfg.init('server.host', 'localhost')
cfg.init('server.port', 8080)

parser = argparse.ArgumentParser()
parser.add_argument('-O', dest='options', action='append',
  metavar='<key>:<value>', help='Overrides an option in the config file')
  
args = parser.parse_args(['-O', 'server.port:9090'])

cfg.update(opt.split(':') for opt in args.options)

print(cfg['server.port'])


for k in cfg:

args = parser.parse_args(['-O', 'port:9090'])
cfg.section('server').update(opt.aplite(':') for opt in args.options)

lock = lockfile.FileLock('.cfglock')
with lock:

import json
s = json.dumps(cfg.as_dict())
cfg.update(json.loads(s))



```

```
```

```
```


