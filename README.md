# react-bugs-solution
### 1. Bug(when running: npm run eject)
```sh
Remove untracked files, stash or commit any changes, and try again.
npm ERR! code 1
npm ERR! path /home/bjit/basic-burger
npm ERR! command failed
npm ERR! command sh -c react-scripts eject

npm ERR! A complete log of this run can be found in:
npm ERR! /home/bjit/.npm/_logs/2021-02-11T06_19_38_305Z-debug.log
```

#### Solution:
```sh
git add .
git commit -am "Save before ejecting"

```
##### or
```sh
rm -rf ~/.git
```
### 2. Bug(Error while installing react-redux)
#### These type of error may be triggered
```sh
* __WEBPACK_IMPORTED_MODULE_4_react___default.a.memo is not a function
* TypeError: Object(...) is not a function
* TypeError: __WEBPACK_IMPORTED_MODULE_0_react___default.a.createContext is not a function
```
#### Solution
```sh
npm install --save react@16.6.0 react-dom@16.6.0
npm install --save react-redux@5.1.1

```

### 3. Bug(Error while installing reactstrap)
#### These type of error may be triggered
```sh
pm ERR!  code ERESOLVE
npm ERR!  ERESOLVE unable to resolve dependency tree
npm ERR! 
npm ERR!  Found: react@17.0.1
npm ERR!  node_modules/react
npm ERR!  peer react@"*" from @testing-library/react@11.2.2
npm ERR!  node_modules/@testing-library/react
npm ERR!  @testing-library/react@"^11.2.2" from the root project
npm ERR!  peer react@"17.0.1" from react-dom@17.0.1
npm ERR!  node_modules/react-dom
npm ERR!  peer react-dom@"*" from @testing-library/react@11.2.2
npm ERR!  node_modules/@testing-library/react
npm ERR!  @testing-library/react@"^11.2.2" from the root project
npm ERR!  react-dom@"^17.0.1" from the root project
npm ERR!  2 more (reactstrap, react-transition-group)
npm ERR!  5 more (the root project, react-icons, react-toastify, ...)
npm ERR! on
```
#### Solution
```sh
npm install reactstrap --legacy-peer-deps

```



