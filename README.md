Electron desktop app for Eclipse Che clients. Generate native platform execuatables that will launch Electron desktop applications that will connect to Eclipse Che or Codenvy servers.

# Download Packaged Executables
1. [Linux x64](https://github.com/TylerJewell/che-electron/releases/download/4.0.0-beta/eclipse-che-electron-linux64.zip)
2. [Linux x32](https://github.com/TylerJewell/che-electron/releases/download/4.0.0-beta/eclipse-che-electron-linux32.zip)
3. [Windows x64](https://github.com/TylerJewell/che-electron/releases/download/4.0.0-beta/eclipse-che-electron-win64.zip)
4. [Windows x32](https://github.com/TylerJewell/che-electron/releases/download/4.0.0-beta/eclipse-che-electron-win32.zip)
5. OSX: You need to currently build the client natively (see build instructions below).

# Run App on Command Line

### Windows
```sh
eclipse-che . <che-server-url>
```

### Mac
```sh
open eclipse-che.app --args . http://localhost:8080
```

### Linux
```sh
./eclipse-che . <che-server-url>
```

# Build Executables From Source
```sh
# Install dependencies
npm install electron-packager -g

git clone http://github.com/tylerjewell/che-electron
cd che-electron && npm run pack:all
```

Optionally, you can build the executable just for your platform.
```sh
npm run pack:win64
npm run pack:win32
npm run pack:linux64
npm run pack:linux32

## If building on windows, this command will fail if console is not run as administrator
npm run pack:osx
```
