# flask-oauth

Flask WSGI tool example with OAuth: <https://wikitech.wikimedia.org/wiki/Help:Toolforge/My_first_Flask_OAuth_tool>

Requires an OAuth consumer grant from <https://meta.wikimedia.org/wiki/Special:OAuthConsumerRegistration/propose>
and a `config.yaml` file with the contents:

```yaml
GREETING: Goodnight moon!
SECRET_KEY: <random secret string>
OAUTH_MWURI: https://meta.wikimedia.org/w/index.php
CONSUMER_KEY: <consumer token>
CONSUMER_SECRET: <consumer secret token>
```

For `SECRET_KEY`, try using the results of `python -c "import os; print repr(os.urandom(24))"`.
