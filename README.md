# LSY CNT landscape based upon official CNCF landscape

![Build and Deploy](https://github.com/lhsystems/landscape/workflows/Build%20and%20Deploy/badge.svg?branch=master)

The Lufthansa Systems Landscape App shows the CNCF-style landscape app with a filtered view with technologies that we use.

## Build time requirements

* NodeJS
* NPM
* YARN

## Runtime requirements

* None (static website)

## How-To

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

## Contributing

Please check out the [contributing guideline](CONTRIBUTING.md) before sending a pull request!