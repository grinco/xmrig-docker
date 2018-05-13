xmrig-docker
============

Docker image for the `xmrig` Monero CPU miner. `xmrig` is built directly from master branch on its public Github repository with all defaults, except devfee which will now default to 0%. You can still opt-in to the devfee from the configuration file.

### Usage
This image is built expecting a JSON configuration file to be available at `$XMRIG_JSON_CONFIG_PATH`. For example, you can mount a volume at `/app/etc` that contains a configuration file named `config.json` with the following command:

```sh
docker run -t -i -d -v /path/to/config/directory:/app/etc -e XMRIG_JSON_CONFIG_PATH=/app/etc/config.json grinco/xmrig:latest
```

### Donations
If this image helped you mine Monero, please feel free to send a donation my way!

* XMR: `43fUjyVCgRpXyTW2eWjfpuTMMJguN44UNi5vs3ogagtkevRaMDqvb7BWbwaVe4vUMveKAzAiA4j8xgUi29TpKXpm3xBaVK9`
 
