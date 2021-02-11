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


