<h1 align="center">
  <br>
    <a href="http://coloredcoins.org">
      <img src="http://coloredcoins.org/img/logo.svg" alt="ColoredCoins" width=200>
    </a>
  <br>
  BankBox
  <br>
  <br>
</h1>

<h4 align="center">ColoredCoins desktop wallet application for digital currency issuance and management.</h4>

<p align="center">
  <a href="http://slack.coloredcoins.org"><img src="http://slack.coloredcoins.org/badge.svg" alt="slack"></a>
</p>

## Screenshots

<p align="center">
  <img src="http://coloredcoins.org/img/bankbox-screenshot-dashboard.JPG" alt="screenshot" height="750" align="center">
  <div style="margin-bottom: 16px;"/>
  <img src="http://coloredcoins.org/img/bankbox-screenshot-transaction.JPG" alt="screenshot" height="750" align="center">
</p>

## Dependencies

BankBox has dependencies on [ColoredCoins full-node](https://github.com/Colored-Coins/Full-Node), which in its turn is dependant on [Bitcoin-Core](https://bitcoin.org/en/bitcoin-core/) and [Redis](https://redis.io/).<br>
Windows installer will download all of those for you, other operating systems will require to download them independently.

## Configuration

BankBox comes with default properties - such as the Bitcoin network (mainnet or testnet), default transaction fee and the configuration for the ColoredCoins full-node server, Bitcoin-Core daemon and Redis. <br>
BankBox `properties.conf` can be found and edited in: <br>
`%APPDATA%\BankBox` (windows) <br>
ColoredCoins full-node `properties.conf`: <br>
`%APPDATA%\coloredcoins-full-node` (windows)

## How to Contribute

### Get the code

```sh
$ git clone https://github.com/Colored-Coins/BankBox.git
$ cd BankBox
$ npm install
```

### Run the app

```sh
$ npm start
```

### Watch the code

Restart the app automatically every time code changes. Useful during development.

```sh
$ npm run watch
```

### Package the app

Builds app binaries. Currently, only Windows is available.

```sh
$ npm run package -- [options]
```

For `[options]` the following optional arguments are available:

- `--sign` - Sign the application
- `--package=[type]` - Package single output type.
  - `exe` - Windows installer
  - `portable` - Windows portable app
  - `all` - All available package options

## Support

You can find support at our [Slack channel](http://slack.coloredcoins.org), or e-mail us to contact@coloredcoins.org.

## License

[AGPL-3.0](https://www.gnu.org/licenses/agpl-3.0.en.html)

