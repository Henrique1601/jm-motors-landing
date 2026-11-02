# 🏛️ Registro de Decisões Arquiteturais (ADRs)

Este documento registra as decisões estratégicas tomadas para o projeto JM Motors.

---

## ADR-001: Stack Base com TanStack Start, Vite 8 e Tailwind CSS v4
* **Contexto:** Necessidade de SSR ultrarrápido para indexação de SEO no Google e animações suaves de produto.
* **Decisão:** Manter TanStack Start com roteamento tipado, Vite 8 com Nitro e Tailwind v4 com tokens OKLCH.
* **Impacto:** Alta pontuação no Core Web Vitals e renderização rápida sem hidratação quebrada.

---

## ADR-002: Renomeação do Repositório para `jm-motors-landing`
* **Contexto:** O projeto foi iniciado como `ride-shine-landing` no Lovable, causando divergência com a marca JM Motors.
* **Decisão:** Renomear oficialmente no GitHub para `Henrique1601/jm-motors-landing` via GitHub CLI, atualizando origin, README e package.json.
* **Impacto:** Consistência de marca, SEO no GitHub e metadados profissionais.

---

## ADR-003: Integração do Estoque Real via Perfil Oficial da OLX
* **Contexto:** O catálogo era estático/mockado com ícones provisórios.
* **Decisão:** Extrair os 12 anúncios ativos do perfil verificado da JM Motors na OLX (`jm-motors-4facad49`), baixar imagens em alta resolução para `public/motos/` com fallback para a CDN da OLX, e centralizar os dados tipados em `src/data/bikes.ts`.
* **Impacto:** O site passa a exibir veículos reais com preços, anos, quilometragens, fotos do showroom e links diretos para negociação.
