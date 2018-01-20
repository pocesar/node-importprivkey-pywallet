# importprivkey-pywallet

Simple script that calls curl in sequence to import pywallet dumpwallet json to Bitcoin (and forks) clients.
It creates meaningless labels for each privkey as `Index ${index}`

## Usage

After using bitcoin.conf and opening the RPC on your client (or daemon), make sure to set the parameters of the command line. Remember to unlock your wallet through "Settings" > "Unlock wallet" else you'll receive an `exit code 22`

```bash
npm install importprivkey-pywallet -g
importprivkey-pywallet --dump ./file.json --user user:pass --url http://127.0.0.1:8332/
```

## External requirements

* Curl
* Node.js 8+
* Dump from [pywallet](https://github.com/jackjack-jj/pywallet)

## License

MIT