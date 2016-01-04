Electron desktop app for Eclipse Che clients. Generate native platform execuatables that will launch Electron desktop applications that will connect to Eclipse Che or Codenvy servers.

# Create Executables
```sh
# Install dependencies
npm install electron-packager -g

git clone http://github.com/tylerjewell/che-electron
npm run pack:all
```

Optionally, you can build the executable just for your platform.
```sh
npm run pack:win64
npm run pack:win32
npm run pack:linux64
npm run pack:linux32
npm run pack:osx
```


# Run App

### Windows
```sh
cd dist\eclipse-che-win32-ia32\
cd dist\eclipse-che-win32-x64\
eclipse-che . <che-server-url>
```

### Mac
```sh
cd dist\eclipse-che-darwin-x64\
open eclipse-che.app . <che-server-url>
```

### Linux
```sh
cd dist\eclipse-che-linux-ia32\
cd dist\eclipse-che-linux-x64\
./eclipse-che . <che-server-url>
```
