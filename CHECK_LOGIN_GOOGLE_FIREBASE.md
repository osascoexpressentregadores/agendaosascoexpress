# Login Google Firebase

Versão ajustada para o admin entrar de duas formas:

1. Entrar com Google
2. Entrar com e-mail e senha

Importante:
- O Google precisa estar ativado em Firebase Authentication > Método de login.
- O domínio do GitHub Pages precisa estar em Authentication > Configurações > Domínios autorizados.
- O e-mail Google usado no login precisa estar liberado nas regras do Firestore para salvar a escala.

Exemplo de regra:

rules_version = '2';

service cloud.firestore {
  match /databases/{database}/documents {
    match /agendas/agenda_reservada_oe {
      allow read: if true;
      allow write: if request.auth != null
        && request.auth.token.email in [
          "SEU_EMAIL_GOOGLE_AQUI"
        ];
    }
  }
}
