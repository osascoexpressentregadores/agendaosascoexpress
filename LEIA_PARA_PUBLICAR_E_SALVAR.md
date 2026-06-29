# Como salvar a escala do admin

Este site é estático. O admin salva primeiro no navegador atual usando localStorage. Isso permite testar na hora no mesmo aparelho.

Para a escala aparecer para todos os entregadores:

1. Entre no Admin.
2. Faça as alterações.
3. Clique em **Baixar HTML atualizado**.
4. Substitua o arquivo **index.html** publicado no GitHub Pages por esse novo arquivo.
5. Abra o link com `?v=novo` no final para forçar atualização no celular.

A versão nova limpa caches antigos automaticamente quando muda o APP_BUILD.
