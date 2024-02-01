# Gerando APK (Android) e IPA (iOS) com React Native & Expo
- Documentação da expo: https://docs.expo.dev/classic/building-standalone-apps/

# Iniciando projeto com expo
- expo init generating-apk

# Modificando app.json adicionando o nome do nosso package
```json
"platforms":[
      "ios",
      "android"
    ],
"android": {
      "package": "com.arthurart.generating-apk"
    },
"ios": {
      "supportsTablet": true,
      "bundleIdentifier": "com.arthurart.generatingapk"
    }
```
# Configurando Android Studio
- https://react-native.rocketseat.dev/
# Building app
- expo build:android ou expo build:ios
- npm install -g eas-cli
- eas build -p android
- Após realizar o comando de gerar apk será necessário gerar o keystore
- Selecione a option Generate new keystore para que o expo gere uma chave
- após terminar o build, basta acessar o link no terminal para baixar a apk.
