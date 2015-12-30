Electron desktop app for Eclipse Che clients. Generate native platform execuatables that will launch Electron desktop applications that will connect to Eclipse Che or Codenvy servers.

# Create Executables
git clone http://github.com/tylerjewell/che-electron

npm run pack:all

# Run App

### Windows
cd dist\eclipse-che-win32-ia32\

cd dist\eclipse-che-win32-x64\

eclipse-che . <che-server-url>

### Mac
cd dist\eclipse-che-darwin-x64\

open eclipse-che.app . <che-server-url>

### Linux
cd dist\eclipse-che-linux-ia32\

cd dist\eclipse-che-linux-x64\

./eclipse-che . <che-server-url>
