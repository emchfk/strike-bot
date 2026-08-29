<div id="toc">
  <ul align="center" style="list-style: none">
    <summary>
      <h1>
        strike-bot
      </h1>
    </summary>
    <em>Self-hostable python app interacting with the strike.me API for DCA and automated profit-making</em>
  </ul>
</div>

## Description

**STRIKE-BOT** is a self-hostable python app interacting with the [STRIKE](https://strike.me/) API to periodically and automatically create EUR-BTC invoices (DCA), store the buy price and sell when a profit threshold is triggered.

## Features

TODO

## Requirements

You need to have:

* [STRIKE](https://strike.me/) account;
* Active [API](https://docs.strike.me/api-keys/overview) key with invoice issuing rights;
* Somewhere to host the app (a Raspberry PI for example!);
* A [PUSHOVER](https://pushover.net/) account, if you want the notifications.

## Example

TODO

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

Rename the file *.toml.example* to *.toml* and update the parameters:

``` bash
TODO
```

Never commit this file, its contains extremely private data!