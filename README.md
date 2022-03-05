# Notes

To install ganache-cli
```bash
npm install -g ganache-cli
```

Run ganache-cli (keep same keys for each session)

```bash
ganache-cli --deterministic
```
---
Set your private keys and address, and adjust this section appropriately:

```python
## For connecting to ganache
w3 = Web3(Web3.HTTPProvider("http://0.0.0.0:8545"))
chaind_id = 1337
my_address = "0x94B806BB0e455576ea46193D9DBbB08d1cc57Da9"
private_key = os.getenv("PRIVATE_KEY")
```

NETWORK ID (chain_id)
```python
CHAIN_ID = 4 # rikeby test network
CHAIN_ID_LOCAL=1337 # local ganache network
```

To set your private key as an environment variable, create .env file in your project with the PRIVATE_KEY variable

```python
private_key = os.getenv("PRIVATE_KEY")
```

Run 
```bash
python deploy.py
```
