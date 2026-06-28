# CHECK — Versão de produção da Agenda Reservada OE

## Decisão de UX aplicada
A tela do motoca foi simplificada para uma agenda semanal vertical.

Regra final:
1. Data manda.
2. Horário organiza.
3. Local confirma.

## Resultado da busca
Agora, ao buscar um nome como Luiz Guilherme, o sistema mostra:
- Agenda reservada para o motoca
- Resumo da semana
- Quantidade de dias reservados
- Quantidade de locais
- Lista dos locais
- Dias em ordem cronológica
- Dentro de cada dia: horário primeiro, local depois
- Aviso discreto quando houver mais de um local no mesmo dia

## Linguagem removida
Foram removidas linguagens com cara técnica ou de dashboard:
- timeline
- roteiro
- compromisso(s)
- ordem por data

## Linguagem aplicada
- Sua semana
- dias reservados
- locais
- horário
- Confirmar minha agenda no WhatsApp

## WhatsApp
A mensagem final também segue a agenda:
- dia/data
- horário
- local

## Mantido
- Agenda pública
- VIP
- Admin
- Busca por nome
- Pop de suporte quando não encontra reserva
- Nomes curtos
- Exportar/importar JSON
- localStorage com chave nova
- Título visual em 2 linhas, preto com destaque vermelho

## Status
Pronta para teste final antes de subir em produção.
