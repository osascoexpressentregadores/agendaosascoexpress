# CHECK — Privacidade e Pontos VIP

## O que foi ajustado
- Removido da navegação pública o acesso direto a Pontos e Gestão.
- A navegação principal agora mostra apenas:
  - Agenda
  - VIP
  - Admin
- A primeira tela não exibe mais números operacionais que possam expor volume, pontos ou equipe.
- Pontos e Gestão continuam existindo internamente, mas ficam fora da navegação pública.
- Após login admin, aparecem atalhos internos para ver pontos e gestão.

## Pontos VIP
- Criada área “Pontos VIP”.
- Mostra mais pontos como bloqueados, sem revelar nomes reais de clientes.
- Para abrir, precisa de código VIP.
- Código padrão: OE2026

## Observação de segurança
Por ser GitHub Pages estático, o código VIP é uma camada visual/prática, não segurança real contra alguém técnico inspecionando o código.
Para segurança real, precisa backend com autenticação.
