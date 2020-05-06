
- npm install electron -g
- cd electronwebviewsample
- npm install # npm install --save-dev electron-builder 와 같이 최신 버전 설치하면 ... 안 됨 
- electron .

# Window OS Build 
- npm run build:win

# Mac OS Build 
- npm install electron-packager -g
- npm install electron-installer-dmg -g

- electron-packager . --overwrite --platform=darwin --arch=x64 --prune=true --out=release-builds # Oni.app 폴드 생성 
- electron-installer-dmg ./release-builds/Oni-darwin-x64/Oni.app Oni --out=release-builds --overwrite # Oni.dmg 설치 파일 생성 

- https://github.com/cba85/electron-webview
