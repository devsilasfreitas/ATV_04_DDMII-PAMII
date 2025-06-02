# firebasechat

Uma aplicação móvel desenvolvida com React Native, Expo, Firebase e NativeWind.

## Tecnologias Utilizadas

- **React Native** - Framework para desenvolvimento mobile
- **Expo** - Plataforma para desenvolvimento React Native
- **Firebase** - Backend as a Service (autenticação, banco de dados, storage)
- **NativeWind** - Framework CSS utilitário para React Native

## Pré-requisitos

Antes de começar, certifique-se de ter instalado em sua máquina:

- [Node.js](https://nodejs.org/) (versão 16 ou superior)
- [npm](https://www.npmjs.com/) ou [Yarn](https://yarnpkg.com/)
- [Expo CLI](https://docs.expo.dev/get-started/installation/)

```bash
npm install -g @expo/cli
```

## Instalação

1. **Clone o repositório**
```bash
git clone https://github.com/seu-usuario/nome-do-projeto.git
cd nome-do-projeto
```

2. **Instale as dependências**
```bash
npm install
# ou
yarn install
```

3. **Instale as dependências específicas do projeto**

### Firebase
```bash
npm install firebase
# ou
yarn add firebase
```

### NativeWind
```bash
npm install nativewind
npm install --save-dev tailwindcss@3.3.2
# ou
yarn add nativewind
yarn add --dev tailwindcss@3.3.2
```

### Dependências adicionais do Expo
```bash
npx expo install expo-dev-client
# ou outras dependências específicas do seu projeto
```

## Configuração

### Firebase
1. Crie um projeto no [Firebase Console](https://console.firebase.google.com/)
2. Adicione uma aplicação web ao seu projeto
3. Copie as credenciais de configuração
4. Crie um arquivo `.env` na raiz do projeto:

```env
EXPO_PUBLIC_FIREBASE_API_KEY=sua_api_key
EXPO_PUBLIC_FIREBASE_AUTH_DOMAIN=seu_projeto.firebaseapp.com
EXPO_PUBLIC_FIREBASE_PROJECT_ID=seu_projeto_id
EXPO_PUBLIC_FIREBASE_STORAGE_BUCKET=seu_projeto.appspot.com
EXPO_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=123456789
EXPO_PUBLIC_FIREBASE_APP_ID=1:123456789:web:abcdef
```

### NativeWind
Certifique-se de que o arquivo `tailwind.config.js` está configurado:

```javascript
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./App.{js,jsx,ts,tsx}", "./src/**/*.{js,jsx,ts,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

## Executando o projeto

1. **Inicie o servidor de desenvolvimento**
```bash
npx expo start
# ou
yarn expo start
```

2. **Execute no dispositivo/emulador**
- Para Android: Pressione `a` no terminal ou escaneie o QR code com o app Expo Go
- Para iOS: Pressione `i` no terminal ou escaneie o QR code com a câmera do iPhone

## 📁 Estrutura do Projeto

```
projeto/
├── src/
│   ├── components/     # Componentes reutilizáveis
│   ├── app(app)/       # Telas da aplicação
│   ├── utils/          # Funções utilitárias
├── assets/             # Imagens e recursos
├── .env                # Variáveis de ambiente
├── app.json            # Configuração do Expo
├── babel.config.js     # Configuração do Babel
├── tailwind.config.js  # Configuração do TailwindCSS
└── package.json        # Dependências do projeto
```

## Funcionalidades Firebase

- **Autenticação**: Login/registro de usuários
- **Firestore**: Banco de dados NoSQL

## Estilização com NativeWind

Este projeto utiliza NativeWind para estilização, que permite usar classes do Tailwind CSS diretamente nos componentes React Native:

```jsx
<View className="flex-1 justify-center items-center bg-blue-500">
  <Text className="text-white text-xl font-bold">
    Hello NativeWind!
  </Text>
</View>
```
---

**Qualquer dúvida entre em contato pelo Teams** 
