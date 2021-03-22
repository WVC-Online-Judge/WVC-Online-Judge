# WVC-Online-Judge

The [Qingdao University Online Judge](https://github.com/QingdaoU/OnlineJudge) system with a customized frontend for West Valley College.

## Dev Environment
### Linux
```bash
cd OnlineJudgeFE
npm install
# we use webpack DllReference to decrease the build time,
# this command only needs execute once unless you upgrade the package in build/webpack.dll.conf.js
export NODE_ENV=development 
npm run build:dll

# the dev-server will set proxy table to your backend
export TARGET=http://Your-backend

# serve with hot reload at localhost:8080
npm run dev
```
### Windows
```batch
cd OnlineJudgeFE
npm install
# we use webpack DllReference to decrease the build time,
# this command only needs execute once unless you upgrade the package in build/webpack.dll.conf.js
set NODE_ENV=development 
npm run build:dll

# the dev-server will set proxy table to your backend
set TARGET=http://Your-backend

# serve with hot reload at localhost:8080
npm run dev
```