# Versão final — Planilha oficial + Firebase Google

Fonte aplicada: `ESCALA COMPLETA OE(4).xlsx`, primeira aba `GERAL - SEMANA`.

## O que foi atualizado

- Escala padrão do site substituída pela planilha oficial atual.
- Login admin via Google configurado com os 4 e-mails autorizados.
- Firebase config do projeto `agendaosascoexpress` inserido no `index.html`.
- Firestore continua no caminho `agendas / agenda_reservada_oe`.
- Proteção contra escala antiga: se o Firestore ainda tiver uma agenda de versão anterior, o site ignora até o admin salvar a escala oficial nova.
- Layout e fluxo existentes foram preservados. Nada foi refeito do zero.

## E-mails admin liberados

- osascoexpress61@gmail.com
- osascoexpressoficial@gmail.com
- operacaoosascoexpress@gmail.com
- bruna.caroline.funari@gmail.com

## Source version

`escala_oficial_geral_semana_fc56d4d6ef9a`

## Publicação

Suba apenas o `index.html` desta pasta no GitHub Pages. Depois abra o site, entre em Admin com Google autorizado e clique em salvar para gravar a versão oficial no Firestore.
