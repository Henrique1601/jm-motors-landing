# ⚠️ Armadilhas Conhecidas & Soluções (Gotchas)

Lições aprendidas e soluções consolidadas para evitar regressões técnicas.

---

### 1. Formato de URLs de Imagens da OLX
* **Gotcha:** `b.imageList` da OLX retorna `path` no formato `/80/802613469618114.jpg`. Montar simplesmente `baseUrl + path` gera 404 porque a CDN exige o prefixo `/images/` ou `/thumbs256x256/`.
* **Solução:** O link correto em alta resolução é `https://img.olx.com.br/images/${path}`. Para resiliência máxima, os arquivos foram baixados localmente para `/public/motos/` com fallback via `onError` no React.

### 2. Bloqueio Anti-Bot da OLX em Fetch Simples
* **Gotcha:** Requisições via `fetch` HTTP direto do Node.js recebem 403 Forbidden do Cloudflare/Datadome.
* **Solução:** `curl.exe` com User-Agent de navegador moderno consegue acessar o payload SSR `__NEXT_DATA__` perfeitamente, permitindo sincronização futura do estoque quando necessário.

### 3. Conexão Lovable & Regra de Não Reescrever Histórico
* **Gotcha:** Fazer `git push -f`, rebase ou squash em commits já enviados quebra o histórico sincronizado com o editor Lovable.
* **Solução:** Apenas commits convencionais incrementais (`git commit`) e pushes normais (`git push origin main`).
