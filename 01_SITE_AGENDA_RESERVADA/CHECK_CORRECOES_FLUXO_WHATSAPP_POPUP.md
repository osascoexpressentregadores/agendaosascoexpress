# CHECK — Correções de fluxo, popup e WhatsApp

Correções aplicadas nesta versão:

1. WhatsApp de confirmação virou mensagem curta, sem quebra de linha e sem risco de aparecer `\n` no texto.
2. Mensagem final enviada: `Oi, suporte OE. Sou [Nome]. Confirmo minha agenda reservada. Pode contar comigo.`
3. Todos os links de WhatsApp passam por higienização antes do encode, removendo `\n`, quebras reais e espaços duplicados.
4. Busca pública passou a procurar somente nome do motoboy, não cliente, ponto, dia ou horário.
5. O popup não abre mais enquanto a pessoa digita. Ele só abre ao clicar em Ver agenda ou apertar Enter.
6. Nome não encontrado agora mostra popup e também card de fallback na tela com botão Chamar suporte.
7. Pesquisa vazia não abre popup; mostra orientação para digitar o nome.
8. Busca por nomes iguais ou parecidos, como Bruno, mostra opções separadas para o usuário escolher.
9. LocalStorage foi atualizado para nova chave v4, evitando puxar escala antiga salva no celular.
