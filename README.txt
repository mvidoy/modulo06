MODULO06: 3-Criando projeto
npm install -g react-native-cli
yarn add react-native-cli
npx react-native init modulo06

cd android
./gradlew clean

MODULO06: 4-ESLint, Prettier & EditorConfig
apagar o arquivo README.md

Generate.editorconfig
trim_trailing_whitespace = true
insert_final_newline = true
end_of_line = lf

yarn add eslint -D
yarn eslint --init
apagar package-lock-json
yarn
yarn add prettier eslint-config-prettier eslint-plugin-prettier babel-eslint -D

*** TELA BRANCA NO EMULADOR ***
deletar node_modules
npm install
react-native run-android

MODULO06: 5-Configurando Reactotron
yarn add reactotron-react-native

src/config/ReactotronConfig.js
const tron = Reactotron.configure({ host: "192.168.0.35" })
    .useReactNative()
    .connect();

MODULO06: 6-React Navigation
yarn add react-navigation react-native-gesture-handler
react-native link react-native-gesture-handler

yarn add jetifier
npx jetify

npm install @react-native-community/cli-platform-android

MainApplication.java:
//////////////////
import com.swmansion.gesturehandler.react.RNGestureHandlerPackage;

@Override
protected List<ReactPackage> getPackages() {
 return Arrays.<ReactPackage>asList(
 new RNGestureHandlerPackage()
 );
}

         /////////////////////////////////
manda um react-native link react-native-gesture-handler e um react-native run-ios
** estas linhas são complementares àquelas que os Docs do RNGH pedem para incluir

https://kmagiera.github.io/react-native-gesture-handler/docs/getting-started.html

Incluir as linhas recomendadas na documentação:
C:\Users\osvaldo\gostack\modulo06\android\app\src\main\java\com\modulo06\MainActivity.java

yar

react-native start run-android

MODULO06: 8-Styled Components
yarn add styled-components

MODULO06: 9-Estilizando formulário
yarn add react-native-vector-icons
react-native link react-native-vector-icons
https://oblador.github.io/react-native-vector-icons/

MODULO06: 10-Acessando API do Github
yarn add axios

MODULO06: 13-Salvando no storage
 "@react-native-community/async-storage": "^1.5.0",
yarn add @react-native-community/async-storage
react-native link @react-native-community/async-storage

