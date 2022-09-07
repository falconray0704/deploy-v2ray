# 1. Configure for your domain

Specify following variables in `.env` file for your domain.

```bash
      VIRTUAL_PORT: 8000 		# The port same as specify in config_server.json
      VIRTUAL_HOST: "foo.bar.com"	# The (sub)domain of your application.
      VIRTUAL_PAHT='/v2ray'	# The path same as specfiy in config_server.json
```

# 2. Configure v2ray

## 2.1 Set uuid 

Get uuid with following command

```bash
docker run -t --rm v2fly/v2fly-core v2ctl uuid
```

Set the uuid in `config_server.json` file.

# 3.Launch:

```bash
docker compose up -d
```

