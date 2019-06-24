# jormungandr-docker
This repo will provide Dockerfiles to help run a Jormungandr node on the Shelley testnet of the Cardano blockchain.

Currently, the Dockerfile provides a quick and easy way to run a private BFT quick-start node with a default configuration.

## Instructions
Clone and build by running these commands:
```bash
git clone https://github.com/nsticco/jormungandr-docker.git
cd jormungandr-docker
docker build -t jor .
```
Launch in detached mode with:
```bash
docker run -d jor
```
See active containers and find container IDs with:
```bash
docker ps
```
Tail logs with:
```bash
docker logs -f <container_ID>
```
Interactively test commands with:
```bash
docker exec -it <container_ID> bash
```

## Reference
[Jormungandr User Guide](https://input-output-hk.github.io/jormungandr/introduction.html)

[Official Jormungandr Repo](https://github.com/input-output-hk/jormungandr)
