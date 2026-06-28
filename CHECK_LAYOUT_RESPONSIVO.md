# Check layout responsivo

## Correções aplicadas
- Layout refeito com grid de 3 áreas: topo, conteúdo e navegação, sem corte.
- Conteúdo de cada tela com rolagem interna segura.
- Largura máxima aumentada para desktop, mantendo boa leitura no celular.
- Cards de dias em `auto-fit`, mudando de várias colunas no desktop para 1 coluna no celular.
- Formulários do admin reorganizados com grid responsivo.
- Linhas do admin quebram para 1 coluna em telas pequenas.
- Botões com altura mínima estável para toque.
- Textos longos com quebra segura e sem estouro lateral.
- Navegação inferior e botão flutuante respeitam safe-area do iPhone.
- Redução de redundância no texto inicial e na explicação do fluxo.
- Botão de contador abre lista de clientes, servindo como atalho sem poluir a UI.

## Pontos de produção
- Sem dependência de backend: alterações continuam salvas no localStorage.
- Para passar alterações para outro dispositivo, usar exportar/importar JSON.
- Se quiser edição global para todos em tempo real, será necessário backend externo.
