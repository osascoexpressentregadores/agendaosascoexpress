# Check login Firebase obrigatório

Correção aplicada:

- Login local antigo `admin / 1212` desativado.
- Chave antiga `oe_agenda_reservada_admin_v1` apagada ao abrir.
- Admin só libera com `firebaseAuth.currentUser`.
- Se Firebase não estiver configurado, o admin fica bloqueado.
- Botão sair faz logout do Firebase.
- A escala só salva para todos quando o admin estiver logado no Firebase.

Se a tela admin abrir sem pedir e-mail/senha, o usuário já está logado no Firebase no navegador.
Nesse caso, clique em Sair e teste novamente.
