# CHECK — Correção de navegação

## Problema percebido
A versão anterior tinha fluxo bom, mas faltavam ações simples que fazem diferença no celular:
- voltar
- topo
- sair do admin
- acesso interno claro após login
- fechamento/retorno mais previsível

## Correções feitas
- Botão Voltar no topo.
- Botão Topo no topo.
- Botões internos de Voltar para agenda e Topo nas páginas.
- Histórico simples de navegação entre abas.
- Admin ganhou barra de saída/retorno.
- Após login admin, aparecem atalhos internos para Pontos e Gestão.
- Botão Sair do admin disponível na barra interna e dentro do admin.
- ESC fecha o pop de suporte em desktop.
- Clique fora do pop de suporte fecha o pop.
- Removido risco de navegação duplicada por múltiplos listeners.

## Mantido
- Agenda reservada.
- Confirmação de compromisso.
- Pop de suporte quando não encontra reserva.
- Pontos VIP com código.
- Admin mobile.
- localStorage.
- Exportar/importar JSON.
