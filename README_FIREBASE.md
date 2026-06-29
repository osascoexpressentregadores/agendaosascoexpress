# Agenda Reservada OE — Versão Firebase

Esta versão salva a escala de verdade para todos usando Firebase + Cloud Firestore.

## O que muda

- GitHub Pages continua servindo o site.
- Cloud Firestore vira o banco online da escala.
- Admin salva no Firebase.
- Entregadores leem a escala atual direto do Firebase.
- O WhatsApp continua simples: `Confirmo meus agendamentos.`

## Passo a passo

1. Acesse o Firebase Console.
2. Crie um projeto.
3. Crie um app Web.
4. Copie o `firebaseConfig`.
5. Abra o `index.html` e substitua este bloco:

```js
const FIREBASE_CONFIG = {
  apiKey: "COLE_AQUI_API_KEY",
  authDomain: "COLE_AQUI_PROJECT.firebaseapp.com",
  projectId: "COLE_AQUI_PROJECT",
  storageBucket: "COLE_AQUI_PROJECT.firebasestorage.app",
  messagingSenderId: "COLE_AQUI_SENDER_ID",
  appId: "COLE_AQUI_APP_ID"
};
```

6. No Firebase, ative Authentication com Email/Senha.
7. Crie um usuário admin.
8. Abra `firestore.rules`, coloque o e-mail admin no lugar de:

```txt
COLOQUE_SEU_EMAIL_ADMIN_AQUI
```

9. No Firebase Firestore, publique as regras.
10. Suba o `index.html` no GitHub Pages.
11. Entre no Admin usando o e-mail e senha do Firebase.

## Estrutura no Firestore

O site grava tudo em:

```txt
agendas / agenda_reservada_oe
```

Campos principais:

- `agenda`: objeto completo da escala
- `updatedAt`: data do salvamento
- `updatedBy`: e-mail do admin

## Primeiro uso

Quando o Firebase estiver configurado, o site começa lendo a escala padrão do HTML.
Depois que o admin fizer a primeira alteração e salvar, o documento será criado no Firestore.
A partir daí, todo mundo passa a ler a escala online.

## Observação importante

Não use mais `localStorage` como fonte oficial.
Com Firebase configurado, a fonte oficial passa a ser o Firestore.


## Status desta versão

O `firebaseConfig` do projeto `agendaosascoexpress` já foi inserido no `index.html`.

Ainda falta configurar no Firebase Console:
1. Authentication com Email/Senha.
2. Criar o usuário admin.
3. Firestore Database.
4. Publicar as regras com o e-mail admin.
