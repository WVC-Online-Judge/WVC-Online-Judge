# WVC-Online-Judge

[![Build](https://github.com/WVC-Online-Judge/WVC-Online-Judge/actions/workflows/build.yaml/badge.svg)](https://github.com/WVC-Online-Judge/WVC-Online-Judge/actions/workflows/build.yaml)

The [Qingdao University Online Judge](https://github.com/QingdaoU/OnlineJudge) system with a customized frontend for West Valley College.

## Production Environment

Run the following commands:

```bash
git clone -b 2.0 https://github.com/WVC-Online-Judge/OnlineJudgeDeploy.git
cd WVC-Online-Judge
docker-compose up -d
```

## Development Environment

Clone the repository recursively (to clone the frontend submodule).

```bash
git clone https://github.com/WVC-Online-Judge/WVC-Online-Judge.git --recursive
cd WVC-Online-Judge
```

When making changes to the frontend, make sure to commit and push both the submodule and the parent repository.

Once you have set up the repo, you can then run the dev server (port 8080).

### Linux

```bash
cd OnlineJudgeFE
npm install
export NODE_ENV=development 
npm run build:dll
export TARGET=http://backend-address:port
npm run dev
```
### Windows

```batch
cd OnlineJudgeFE
npm install
set NODE_ENV=development 
npm run build:dll
set TARGET=http://backend-address:port
npm run dev
```

## Building for Production

Navigate to the [Build GitHub Action](https://github.com/WVC-Online-Judge/WVC-Online-Judge/actions/workflows/build.yaml) and click `Run workflow`.

![image](https://user-images.githubusercontent.com/38841491/121101011-d0ba3300-c7af-11eb-871f-9640235081bd.png)

