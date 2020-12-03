# CNT landscape application/generator forked from official CNCF landscape

## How To Run Locally

Setup
```
# Setup
git clone https://github.com/lhsystems/landscapeapp.git
git clone https://github.com/lhsystems/landscape.git

cd landscapeapp
yarn
```

Creating the landscape
```
export SKIP_VERSION_CHECK=1
export PROJECT_PATH=$(pwd)/../landscape
export GITHUB_KEY=<...>

yarn run build
```

Browsing the landscape
```
cd ../landscape/dist
# Serve this directory by whatever webserver, example:
python3 -m http.server
```


