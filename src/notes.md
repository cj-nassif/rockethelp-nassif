## Notas sobre o projeto
### Iniciando projeto

- [x] expo init rockethelp-nassif
### Dando suporte ao Typescript

- Renomeio o arquivo **App.js** para **App.tsx**
- Crie um arquivo **tsconfig.json**
- Inicie o projeto com o expo com o comando: *"expo start"*

### Biblioteca de componentes para React Native => **NativeBase**

https://nativebase.io/

- Instalação Native base em projeto expo

- [x] yarn add native-base
- [x] expo install react-native-svg
- [x] expo install react-native-safe-area-context

### Expo google fonts

- [x] expo install expo-font @expo-google-fonts/roboto

### Biblioteca para trabalhar com SVG em forma de componente

- react native svg transformer intruções de configuração:

https://github.com/kristerkari/react-native-svg-transformer

- [x] yarn add --dev react-native-svg-transformer

### Snippet extensao VS Code - R Component

- **nbc** => snippet para criação de componentes native base

### Biblioteca de Icones phosphorIcons

https://phosphoricons.com/

- [x] yarn add phosphor-react-native

### Lib Navegação - React Navigation

https://reactnavigation.org/docs/getting-started/

- [x] yarn add @react-navigation/native
- [x] expo install react-native-screens 
- [x] yarn add @react-navigation/native-stack

### Utilizando o Firebase na aplicação

**Não é possível utilizar o expo go com o Firebase**

https://firebase.google.com/

- Entrar no console
- Adicionar projeto
- Nomear o projeto
- Continuar 
- Projeto Pronto

**No projeto será utilizado autenticação, e Firestore database**

#### Autenticação

- Clique na aba autenticação e vamos começar
- Selecione a opção e-mail e senha e *ativar* e *salvar*
- Clique agora na aba *users* e após em *Usuario Novo* 
- Cadastre um e-mail para usuario e senha (a senha deverá ter pelo menos 6 dígitos)
- Adicionar usuário

#### Firestore

- Criação
- Firestore database
- Criar banco de dados
- Iniciar em modo de testes
- Avançar
- Ativar

#### Criando coleção

- Criar coleção
- Nomear coleção **orders**
- Gerar código automático
- Gerar os campos

**Para essa aplicação não será necessário criar manualmente esse coleção pois na hora que for feita a primeira solicitação o firestore irá criar automaticamente essa coleção com base na estrutura da requisição.**

### Habilitando a aplicação para utilizar o firebase

https://rnfirebase.io/

- Seguir o passo a passo da instalação

#### Módulo Principal

- [x] yarn add @react-native-firebase/app

#### Configurar os arquivos de conexão

- Visão geral do projeto
- Adicione um app para começar

*IOS*

- Coloque o nome do pacote
- Crie um apelido (opcional)
- Registrar app
- Fazer o download do arquivo e salvar na raiz do projeto
- Clicar em próximo
- Clicar em próximo
- Clicar em continuar no console

*Android*

- Coloque o nome do pacote
- Crie um apelido (opcional)
- Registrar app
- Fazer o download do arquivo e salvar na raiz do projeto
- Clicar em próximo (Não necessári pois o expo vai cuidar dessas configurações)
- Clicar em próximo (Não necessári pois o expo vai cuidar dessas configurações)
- Clicar em continuar no console

#### Realizar as etapas de configuração no código nativo

**No expo é possível realizar essas configurações através de um plugin**

https://docs.expo.dev/guides/setup-native-firebase/

`
{
  "expo": {
    "plugins": [
      "@react-native-firebase/app"
    ],
    "android": {
      "package": "com.nassif.cj.rockethelpnassif",
      "googleServicesFile": "./google-services.json"
    },
    "ios": {
      "bundleIdentifier": "com.nassif.cj.rockethelpnassif",
      "googleServicesFile": "./GoogleService-Info.plist"
    }
  }
}
`
Rode o comando:

- [x] expo prebuild
#### Módulo Firestore

https://rnfirebase.io/firestore/usage

- [x] yarn add @react-native-firebase/firestore

#### Módulo Autenticação

https://rnfirebase.io/auth/usage

- [x] yarn add @react-native-firebase/auth




