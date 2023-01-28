title: Install Node.js with nvm
tags: []
categories: []
date: 2023-01-28 14:49:00
---
1. install nvm – node version install control
	1.1 view the newest nvm version
    	```
        https://github.com/nvm-sh/nvm/releases
        ```
    1.2 install nvm
    	```
        curl https://raw.githubusercontent.com/creationix/nvm/v0.39.3/install.sh | bash
        ```
    1.3 re-souce
    	```
        source ~/.profile
        ```
    1.4 check
    	```
        nvm --version
        ```
2. install node + npm
	2.1 view the node.js versions
    	```
        nvm ls-remote
    	```
    2.2 install the obejct version nod
    	```
        nvm install v18.13.0
        ```
    2.3 use the object version node
    	```
        nvm use 18.13.0
        ```
    2.4 set to default version
    	```
        nvm alias default 
        ```
    2.5 restart and check
    	```
        node -v
        ```
3. install the newest npm
    	```
		npm install -g npm@latest
    	```
