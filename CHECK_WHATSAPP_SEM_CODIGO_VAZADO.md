# CHECK WHATSAPP SEM CÓDIGO VAZADO

Correção aplicada no fluxo de confirmação do WhatsApp.

## Regra final
A mensagem enviada para o WhatsApp é sempre texto puro em uma única linha.

Mensagem padrão:
Oi, suporte OE. Sou NOME_DO_MOTOBOY. Confirmo minha agenda reservada. Pode contar comigo.

## Proteções aplicadas
- Remove `\\n`, `\\r`, `\\t` antes de montar o link.
- Remove quebras reais de linha antes de montar o link.
- Remove HTML, `<br>`, chaves e sinais de código.
- Remove resíduos `%0A`, `%0D`, `%5Cn`, `%5Cr` caso venham de versão antiga.
- Gera o link sempre com `encodeURIComponent` sobre texto já limpo.
- Intercepta o clique do botão e reconstrói o link na hora do clique.
- Nova chave de localStorage para não reaproveitar versão antiga salva no celular.

## Validação
Bruno Getaruch decodifica exatamente como:
Oi, suporte OE. Sou Bruno Getaruch. Confirmo minha agenda reservada. Pode contar comigo.

Sem `\\n`, sem `%0A`, sem HTML e sem quebra vazada.
