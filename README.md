<p align="center">
  <img width="200" height="200" alt="Logo clean e moderno do _Alimenta Fácil_" src="https://github.com/user-attachments/assets/1a530b00-1bf5-4cc3-a209-e6b7205f2450" />
</p>

<p align="center">
  🚀 Um sistema moderno para organizar compras, refeições, cardápios e controle alimentar.
</p>

---

## 📌 Badges

<div align="center">

![Next.js](https://img.shields.io/badge/Next.js-14-black?logo=next.js)
![TypeScript](https://img.shields.io/badge/TypeScript-5-blue?logo=typescript)
![React](https://img.shields.io/badge/React-19-61dafb?logo=react)
![Tailwind](https://img.shields.io/badge/TailwindCSS-3-38bdf8?logo=tailwind-css)
![Shadcn](https://img.shields.io/badge/Shadcn-UI-000000)
![Status](https://img.shields.io/badge/status-em_desenvolvimento-yellow)
![License](https://img.shields.io/badge/license-MIT-green)

</div>

---

# 🧠 Sobre o Produto

O **Alimenta Fácil** é um aplicativo criado para facilitar o planejamento alimentar e melhorar a experiência de compras e organização doméstica.

Ele permite:

- Organizar lista de compras  
- Registrar e controlar itens alimentares  
- Criar cardápios semanais  
- Controlar estoque e validade  
- Reduzir desperdício  
- Acompanhar gastos com alimentação  
- Gerar sugestões automáticas baseadas no consumo  

O foco é: **economia, praticidade e organização**.

---

# 🧱 Stack Tecnológica

| Área | Tecnologia |
|------|------------|
| Framework | **Next.js 14+ (App Router)** |
| Linguagem | **TypeScript (strict)** |
| UI | **TailwindCSS + Shadcn/UI** |
| Estado | A definir (Zustand / Context / Signals) |
| Qualidade | ESLint, Prettier |
| Versionamento | Git + GitHub Flow |

---

# 🔀 Git Flow do Projeto

O projeto usa um **Git Flow simplificado e eficiente**.

### 🌿 Branches principais
| Branch | Finalidade |
|--------|------------|
| `main` | Código estável, pronto para produção |
| `develop` | Ambiente de desenvolvimento |

### 🚧 Fluxo de Features

develop
↳ feature/nome-da-feature
→ Pull Request → develop


### 📌 Convenções do projeto
- Nada de commits direto em `main` ou `develop`
- Tudo via Pull Request
- Branch de feature deve ser apagada após o merge
- Commits:  
  `feat:`, `fix:`, `docs:`, `refactor:`, `chore:`

<section id="como-rodar-o-projeto">
  <h2>⚙️ Como Rodar o Projeto</h2>

  <h3>🔧 Pré-requisitos</h3>
  <p>Certifique-se de ter instalado:</p>
  <ul>
    <li><strong>Node 20.12.2</strong> (use <code>nvm use</code> para ativar a versão correta)</li>
    <li><strong>npm 10+</strong></li>
    <li>Git</li>
  </ul>

  <p>O projeto possui um arquivo <code>.nvmrc</code>. Ao entrar na pasta do projeto, rode:</p>
  <pre><code>nvm use</code></pre>

  <hr>

  <h3>📦 Instalar dependências</h3>
  <pre><code>npm install</code></pre>

  <hr>

  <h3>🚀 Rodar em ambiente de desenvolvimento</h3>
  <pre><code>npm run dev</code></pre>
  <p>A aplicação ficará disponível em: 
    <a href="http://localhost:3000" target="_blank">http://localhost:3000</a>
  </p>

  <hr>

  <h3>🧪 Verificar tipos (TypeScript)</h3>
  <pre><code>npm run type-check</code></pre>

  <hr>

  <h3>🧱 Criar build de produção</h3>
  <pre><code>npm run build</code></pre>

  <hr>

  <h3>▶️ Rodar versão de produção</h3>
  <pre><code>npm run start</code></pre>

  <hr>

  <h3>🧹 Limpar cache e artefatos de build</h3>
  <pre><code>npm run clean</code></pre>

  <hr>

  <h3>📄 Scripts disponíveis</h3>
  <table>
    <thead>
      <tr>
        <th>Script</th>
        <th>Descrição</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td><code>npm run dev</code></td>
        <td>Inicia o ambiente de desenvolvimento</td>
      </tr>
      <tr>
        <td><code>npm run build</code></td>
        <td>Gera o build de produção</td>
      </tr>
      <tr>
        <td><code>npm run start</code></td>
        <td>Inicia o servidor de produção</td>
      </tr>
      <tr>
        <td><code>npm run type-check</code></td>
        <td>Valida tipos do TypeScript</td>
      </tr>
      <tr>
        <td><code>npm run lint</code></td>
        <td>Executa o ESLint</td>
      </tr>
      <tr>
        <td><code>npm run clean</code></td>
        <td>Limpa cache e arquivos de build</td>
      </tr>
    </tbody>
  </table>
</section>


<!-- LICENÇA -->
<h2>📄 Licença</h2>
<p>Projeto licenciado sob <strong>MIT</strong>.</p>

<p class="center">
  Feito com 💚 para facilitar sua rotina alimentar.
</p>



