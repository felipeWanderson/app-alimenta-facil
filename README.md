# 🍎 Alimenta Fácil

Aplicativo moderno para organização de compras, com listas automáticas baseadas em porções, histórico inteligente e UX minimalista.

## 🚀 Stack Principal

- Next.js 14
- TypeScript
- Tailwind CSS
- shadcn/ui
- Zustand
- Dexie.js (IndexedDB)
- Zod
- React Hook Form
- Playwright + Jest
- CI/CD com GitHub Actions + Vercel

## 📦 Funcionalidades do MVP

- Cadastro de itens (com porção opcional)
- Lista manual
- Lista automática com cálculo e arredondamento inteligente
- Histórico em cards
- Duplicação de listas
- Salvamento local (offline-first)

## 🧱 Arquitetura

- Feature-based structure
- Repository pattern
- Services para regras de negócio
- Schemas centralizados (Zod)
- Estado global por feature (Zustand)

## 📌 Roadmap

Veja os milestones no GitHub Projects.

## ⚙️ CI/CD

- Lint
- Typecheck
- Testes (unit, integration, e2e)
- Build
- Deploy automático na Vercel

## Node Version

Esse projeto usa Node **20.12.2**  
Rode `nvm use` antes de instalar as dependências.
