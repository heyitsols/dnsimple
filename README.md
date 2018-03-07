# dnsimple
A bash script for interacting with your dnsimple account.

## Installation
Requires `jq` in your `bin`. [Download](https://stedolan.github.io/jq/).

Make `dnsimple` executable and move to `bin`.

```bash
chmod +x dnsimple; mv dnsimple /usr/local/bin;
```

### API Key
Get your dnsimple API key by logging in and going to Account > API Tokens > New Access Token. For now, paste it into the script, just make sure you don't commit to version control.

### Account ID
Working on grabbing the account id from a json request. For now, you'll need to provide it at the command line. See usage.

## Usage

For now, just two commands:

### List domains
Returns a list of domains registered or hosted with dnsimple.

```bash
dnsimple -a XXXXX list
```

### Account details
Returns your account details.

```bash
dnsimple -a XXXXX account
```