# nextjs-app
base skeleton


## Get NVM for windows to handle multiple projects with diff node version code bases

https://github.com/coreybutler/nvm-windows#readme
>  nvm --version
> 1.1.12

## Install a node version (lts) 
> nvm install lts 64

 ```
PS C:\Users\satbasu> nvm install lts 64
Downloading node.js version 20.17.0 (64-bit)...
Extracting node and npm...
Complete
npm v10.8.2 installed successfully.


Installation complete. If you want to use this version, type

nvm use 20.17.0
 ```

That's a known issue with nvm on Windows. When you use nvm use to switch to a different version of Node.js, the corresponding version of npm is not automatically updated in your terminal.
This is because nvm only updates the PATH environment variable to point to the new version of Node.js, but it doesn't update the npm command to use the corresponding version of npm.
To fix this issue, you can use the following command to update the npm command to use the corresponding version of npm:

```
nvm use v20.17.0 && npm install -g npm@20.17.0
```
