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

### Setting up application parameters

Rename the file *.toml.example* to *.toml* and update the parameters:

``` bash
TODO
```

Never commit this file, it contains extremely private data!

## Running as service

### Installation

Copy the main script service file to the following location:

``` bash
sudo cp .service /etc/systemd/system/strike-bot.service
```

Reload the systemd configuration:

``` bash
sudo systemctl daemon-reload
```

Activate the automatic start when booting:

``` bash
sudo systemctl enable strike-bot.service
```

Start the service:

``` bash
sudo systemctl start strike-bot.service
```

To check the service status:

``` bash
sudo systemctl status strike-bot.service
```

### Logs

To see the logs in real-time:

``` bash
journalctl -u strike-bot.service -f
```

To see previous logs:

``` bash
journalctl -u strike-bot.service
```

### Checks

To check the service is active:

``` bash
sudo systemctl is-active strike-bot.service
```

This should return *active*.

To check the service is activated at boot:

``` bash
sudo systemctl is-enabled strike-bot.service
```

This should return *enabled*.