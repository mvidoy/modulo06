MODULO06: 3-Criando projeto
yarn add react-native-cli
npx react-native init modulo06
yarn add jetifier -D
npx jetify

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




