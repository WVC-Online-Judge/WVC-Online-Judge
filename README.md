# WVC-Online-Judge

The [Qingdao University Online Judge](https://github.com/QingdaoU/OnlineJudge) system with a customized frontend for West Valley College.

## Dev Environment

The dev build runs on port 8080.

### Linux

```bash
npm install
export NODE_ENV=development 
npm run build:dll
export TARGET=http://backend-address:port
npm run dev
```
### Windows

```batch
npm install
set NODE_ENV=development 
npm run build:dll
set TARGET=http://backend-address:port
npm run dev
```
