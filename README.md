<p align="center">
  <img src="public/og-image.jpg" width="700" alt="JM Motors Santos — Showroom" style="border-radius: 12px; box-shadow: 0 10px 30px rgba(0,0,0,0.5);" />
</p>

# 🏍️ JM Motors — Landing Page Oficial

<p align="center">
  <strong>Concessionária de motos novas e seminovas em Santos/SP · Vila Mathias</strong>
</p>

<p align="center">
  <a href="https://github.com/Henrique1601/jm-motors-landing/releases"><img src="https://img.shields.io/badge/version-v1.0.0-blue.svg?style=for-the-badge" alt="Version"></a>
  <a href="https://react.dev"><img src="https://img.shields.io/badge/React-19.2.0-61DAFB.svg?style=for-the-badge&logo=react&logoColor=black" alt="React 19"></a>
  <a href="https://tanstack.com/start"><img src="https://img.shields.io/badge/TanStack_Start-1.168-FF4154.svg?style=for-the-badge" alt="TanStack Start"></a>
  <a href="https://tailwindcss.com"><img src="https://img.shields.io/badge/Tailwind_CSS-v4.2-38B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white" alt="Tailwind CSS"></a>
  <a href="LICENSE"><img src="https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge" alt="License: MIT"></a>
  <a href="https://lovable.dev"><img src="https://img.shields.io/badge/Lovable-Connected-FF3366.svg?style=for-the-badge" alt="Lovable"></a>
</p>

<p align="center">
  <a href="#-visão-geral">Visão Geral</a> •
  <a href="#-recursos-e-alavancas-de-conversão">Recursos</a> •
  <a href="#-stack-tecnológica">Tecnologias</a> •
  <a href="#-seo-local--dados-estruturados">SEO Local</a> •
  <a href="#-como-executar-localmente">Execução Local</a> •
  <a href="#-build-with-lovable">Lovable</a> •
  <a href="#-licença">Licença</a>
</p>

---

## 📌 Visão Geral

A **JM Motors** é uma landing page comercial de alto padrão projetada para impulsionar a atração e captação de clientes para a concessionária física localizada na **Av. Senador Feijó, 455 — Vila Mathias, Santos - SP**.

Construída sobre uma estética dark industrial contemporânea (OKLCH, tipografia de impacto *Big Shoulders Display* e *DM Sans*), a aplicação combina **SSR ultrarrápido** com **motion physics fluido**, entregando carregamento instantâneo, alta conversão mobile e integração direta com o WhatsApp dos consultores de venda.

---

## ⚡ Recursos & Alavancas de Conversão

- **🏍️ Catálogo Dinâmico de Motos:** Vitrine categorizada com filtros interativos por montadora (Honda, Kawasaki, Scooters, Nakeds e Esportivas).
- **🧮 Simulador de Financiamento em Tempo Real:** Calculadora interativa permitindo ao cliente simular valor do veículo, entrada (incluindo opção sem entrada) e parcelamento (24x, 36x, 48x), com botão de envio direto do cálculo pré-formatado para o WhatsApp.
- **🔄 Módulo "Avalie sua Usada na Troca":** Fluxo em 3 etapas para avaliação de seminovas com pré-avaliação rápida via WhatsApp.
- **⭐ Carrossel de Avaliações Google:** Carrossel responsivo com suporte a swipe mobile, autoplay suave e pausa ao passar o mouse, conectado à base de dados centralizada (`src/data/testimonials.ts`) com link oficial para novas avaliações no Google Meu Negócio.
- **📱 Menu Mobile Responsivo (Drawer):** Navegação fluida e acessível adaptada para smartphones e tablets.
- **❓ FAQ Accordion:** Sanando dúvidas frequentes de procedência, laudo cautelar, garantia de motor/câmbio e localização da loja física.
- **🗺️ Geo-Localização e Horários:** Integração com Google Maps da Vila Mathias, horários semanais e fins de semana e link de rota direta.

---

## 🔍 SEO Local & Dados Estruturados

A aplicação conta com infraestrutura completa de SEO técnico e regional para Santos e Baixada Santista:

- **Schema.org `MotorcycleDealer` (JSON-LD):** Metadados estruturados com nome, endereço na Av. Senador Feijó, coordenadas geográficas (latitude/longitude), horário de atendimento e cidades atendidas (*Santos, São Vicente, Praia Grande, Guarujá, Cubatão*).
- **Schema.org `FAQPage`:** Perguntas e respostas formatadas para Rich Snippets na SERP do Google.
- **Open Graph & Twitter Cards:** Card visual otimizado em 16:9 (`og-image.jpg`) para previews no WhatsApp, Instagram e redes sociais.
- **Sitemap XML & Robots.txt:** `sitemap.xml` dinâmico mapeando todas as âncoras e `robots.txt` indexável.

---

## 🛠️ Stack Tecnológica

| Camada | Tecnologia | Propósito |
|---|---|---|
| **Framework Full-Stack** | [TanStack Start](https://tanstack.com/start) + [Nitro](https://nitro.unjs.io/) | Server-Side Rendering (SSR) e roteamento seguro |
| **Bundler & Tooling** | [Vite 8](https://vitejs.dev/) | HMR ultraveloz e builds otimizados |
| **UI Library** | [React 19](https://react.dev/) | Componentização moderna e hooks nativos |
| **Estilização** | [Tailwind CSS v4](https://tailwindcss.com/) | Design tokens baseados em OKLCH e CSS puro |
| **Animações** | [Motion](https://motion.dev/) | Microinterações, transições de layout e parallax |
| **Ícones** | [Lucide React](https://lucide.dev/) | Ícones vetoriais leves e consistentes |
| **Deploy** | [Vercel](https://vercel.com/) | Edge deployment com CI/CD contínuo via GitHub |

---

## 💻 Como Executar Localmente

### Pré-requisitos
- **Node.js** 20+ ou 24+ instalado
- Gerenciador de pacotes **npm** ou **bun**

### Instalação e Execução

```sh
# 1. Clone o repositório
git clone https://github.com/Henrique1601/jm-motors-landing.git
cd jm-motors-landing

# 2. Instale as dependências
npm install

# 3. Inicie o servidor de desenvolvimento
npm run dev
```

Acesse [http://localhost:3000](http://localhost:3000) no seu navegador.

### Outros Scripts

```sh
npm run build      # Compilação de produção com Nitro/Vite
npm run preview    # Visualização local do build compilado
npm run lint       # Auditoria de código via ESLint
npm run format     # Formatação de código via Prettier
npm run test       # Execução da suíte de testes com Vitest
```

---

## 🔄 Como Adicionar Novas Avaliações do Google

Para adicionar novos depoimentos ao carrossel da loja, basta editar o arquivo [`src/data/testimonials.ts`](src/data/testimonials.ts) e incluir um novo registro:

```ts
{
  id: "7",
  name: "Nome do Cliente",
  city: "Santos - SP",
  bike: "Honda PCX 160",
  rating: 5,
  date: "Há 2 dias",
  text: "Texto da avaliação deixada no Google...",
}
```

O carrossel recalcula os slides e a navegação automaticamente.

---

## 🎨 Build with Lovable

This project was synchronized and developed with [Lovable](https://lovable.dev/projects/46b05c47-a4ff-4912-a5b9-74284ef8becb).

- **Full ownership**: Every change made locally or in Lovable is synchronized seamlessly via GitHub.
- **Git workflow**: Push to `main` on GitHub and changes are deployed to Vercel and reflected in Lovable.

---

## 📄 Licença

Distribuído sob a licença **MIT**. Consulte o arquivo [`LICENSE`](LICENSE) para mais detalhes.

Copyright (c) 2026 **Henrique Bezerra Dos Santos**.
