
## Export Required Variables

```bash
export REGISTRY1_USERNAME=rob.ferguson
export REGISTRY1_PASSWORD=<password>

# Used for BigBang scripts
export BIGBANG_DIR=/home/rob/du/bigbang
export DRIVER_BIGBANG_DIR=/home/rob/du/driver-bigbang

# Setting default kubeconfig to bigbang driver kubeconfig
# Can optionally set this manually
export KUBECONFIG=/home/rob/du/driver-bigbang/kubeconfig.yaml
```

## Big Bang Driver
```bash
mkdir -p $DRIVER_BIGBANG_DIR/overrides/neuvector
touch $DRIVER_BIGBANG_DIR/overrides/neuvector/values.yaml # Edit this to override values

bb --host 192.168.1.163 --nodes 3 --sso --package neuvector
```
