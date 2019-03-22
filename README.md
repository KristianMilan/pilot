# Yazz
### Build Docker Webapps in Minutes (Beta)

- Build apps in minutes with drag and drop interface and code business logic in Javascript
- One click deploy to Docker
- Open source MIT license
- Runs in Docker on the cloud or locally
- Can be run as a Desktop app in Electron

http://yazz.com

Quick start:
- Download and run Docker

- Expose the Docker REST api with:
    `docker run -d -v /var/run/docker.sock:/var/run/docker.sock -p 127.0.0.1:1234:1234 bobrik/socat TCP-LISTEN:1234,fork UNIX-CONNECT:/var/run/docker.sock`
    
- Install and run the Yazz IDE with:
    `docker run -p 80:80 zubairq/yazz`
    
- Go to a browser and view Yazz:
    http://localhost
    




Command line options :

    -h, --help                 output usage information
    -V, --version              output the version number
    -t, --type [type]          Add the specified type of app [type]
    -p, --port [port]          Which port should I listen on? [port]
    -h, --host [host]          Server address of the central host [host]
    -s, --hostport [hostport]  Server port of the central host [hostport]



### Developer quick start


##### 1) Install GIT from https://git-scm.com/downloads
##### 2) Install Node.js 8.9 64 bit installer from https://nodejs.org/en/download/
##### 3) From the command line get the Git repository
    git clone https://github.com/zubairq/yazz.git
##### 4) Go to the yazz directory
    cd yazz
##### 5) Install the NodeJS modules
    npm install
##### 6) Install SQlite3 for Electron
    Copy
        node_macos64/node_sqlite3.noderename
    to
        node_modules/sqlite3/lib/binding/node-v57-darwin-x64/node_sqlite3.node
##### 7) Run the Yazz Electron application
    electron .



### To build the Mac .app you also need to
##### 1) Install SQlite3 for Electron
    sudo npm install sqlite3 --build-from-source --runtime=electron --target=1.8.4 --dist-url=https://atom.io/download/electron (this step may not be needed on some platforms)
##### 2) Run electron packager
    Sudo electron-forge make



### What is Yazz's killer feature?

Yazz's killer feature is being able to build simple internal business apps fast. It enables this by allowing all apps to be made with our drag and drop editor and the Javascript and SQL scripting language

### Is there commercial support for Yazz?
If you require commercial support then please go to http://yazz.com
