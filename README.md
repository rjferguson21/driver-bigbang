## Big Bang Driver
```bash
mkdir neuvector-test
cp base/values.yaml neuvector-test

bb --host 192.168.1.163 --nodes 3 --package neuvector
```

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