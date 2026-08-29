<p align="center">
  <a href="https://github.com/emchfk/strike-bot"><img src="docs/img/banner.png" alt="strike-bot"></a>
</p>
<p align="center">
    <em>Self-hostable python app interacting with the strike.me API</em>
</p>

---

**STRIKE-BOT** is a self-hostable python app interacting with the [STRIKE](https://strike.me/) API to periodically and automatically create EUR-BTC invoices, store the buy price and sell when a profit threshold is triggered.

## Requirements

You need to have:

* [STRIKE](https://strike.me/) account;
* Active [API](https://docs.strike.me/api-keys/overview) with invoice issuing rights;
* Somewhere to host the app (a Raspberry PI for example!).

## Setting up

### Setting up Python environment

``` bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

### Updating environment

To update/upgrade pip and detect outdated packages, use the following commands:

``` bash
pip install --upgrade pip
pip list --outdated
```

### Setting up environment variables

Rename the file *.env.example* to *.env* and update the parameters:

``` bash
TODO
```