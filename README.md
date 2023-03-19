# trueblocks-stack
A repo combining Erigon EL, one of the CLs, and the TrueBlocks indexer

Modified from https://github.com/kimpers/lighthouse-docker

1. Clone the repository
```bash
git clone https://github.com/CyMule/trueblocks-stack.git
```
2. Navigate to the cloned repository
```bash
cd trueblocks-stack
```

3. Generate a 32-byte random hex string and save it to a file named "jwt.hex":
```bash
openssl rand -hex 32 | tr -d "\n" > "jwt.hex"
```

4. Make a directory for the erigon-data 
```bash
mkdir erigon-data
```

5. Copy the default.env to .env and edit it as needed:
```bash
cp default.env .env
```

6. Finally, start the Docker Compose stack:
```bash
docker compose up
```
