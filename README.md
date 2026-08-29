<style>
    header {
        display: flex;
        align-items: center;
        padding: 20px;
        justify-content: center;
    }
    .logo {
        margin-right: 20px;
    }
    .logo img {
        max-height: 100px; /* Ajuste la hauteur selon tes besoins */
    }
    .title {
        text-align: center;
    }
    .titleh1 {
        margin: 0;
        font-size: 40px; /* Ajuste la taille selon tes besoins */
    }
</style>

<header>
<div class="logo" align="center">
  <img src="docs/img/strike-logo.png" alt="strike-bot">
</div>
<div class="title" align="center">
    <p class="titleh1">strike-bot</p>
</div>
</header>
<p align="center">
    <em>Self-hostable python app interacting with the strike.me API for DCA and automated profit-making</em>
</p>

## Description

**STRIKE-BOT** is a self-hostable python app interacting with the [STRIKE](https://strike.me/) API to periodically and automatically create EUR-BTC invoices (DCA), store the buy price and sell when a profit threshold is triggered.

## Features

TODO

## Requirements

You need to have:

* [STRIKE](https://strike.me/) account;
* Active [API](https://docs.strike.me/api-keys/overview) with invoice issuing rights;
* Somewhere to host the app (a Raspberry PI for example!).

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