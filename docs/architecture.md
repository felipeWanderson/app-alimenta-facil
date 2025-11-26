<h1>📘 Arquitetura do Projeto — Alimenta Fácil</h1>

<h2>🎯 Objetivo</h2>
<p>
  Estruturar o projeto de forma clara, modular e escalável, garantindo organização, facilidade de manutenção
  e colaboração eficiente entre desenvolvedores.
</p>

<hr />

<h2>📁 Estrutura Geral</h2>

<pre><code>app/
components/
features/
hooks/
lib/
services/
styles/
utils/
</code></pre>

<p>
  Cada pasta possui uma responsabilidade específica, seguindo boas práticas de modularização modernas 
  adotadas por projetos da Vercel, Shopify e grandes times de engenharia.
</p>

<hr />

<h2>📂 app/</h2>
<p><strong>Responsável pelo App Router do Next.js.</strong></p>

<ul>
  <li>layout.tsx</li>
  <li>page.tsx</li>
  <li>Rotas aninhadas</li>
  <li>Server Components</li>
  <li>Metadata</li>
  <li>Server Actions</li>
</ul>

<p><strong>Regra:</strong> Apenas UI de páginas e lógica de roteamento. Nada de regras de negócio aqui.</p>

<hr />

<h2>📂 components/</h2>
<p><strong>Componentes globais e reutilizáveis, independentes de regras de negócio.</strong></p>

<ul>
  <li>Botões</li>
  <li>Inputs</li>
  <li>Modais</li>
  <li>Cards</li>
  <li>Skeletons</li>
  <li>Componentes do Design System</li>
</ul>

<p><strong>Regra:</strong> Se um componente pertence a uma feature, deve ficar em <code>features/</code>.</p>

<hr />

<h2>📂 features/</h2>
<p><strong>Módulos isolados que representam áreas funcionais do sistema.</strong></p>

<pre><code>features/
  shopping-list/
    components/
    services/
    hooks/
    types/
    utils/
</code></pre>

<p>Cada feature deve conter:</p>

<ul>
  <li>Componentes específicos</li>
  <li>Hooks da feature</li>
  <li>Serviços (requisições e regras)</li>
  <li>Tipos e schemas</li>
  <li>Funções utilitárias internas</li>
</ul>

<p><strong>Benefícios:</strong> baixa complexidade, escalabilidade, testabilidade e modularidade.</p>

<hr />

<h2>📂 hooks/</h2>
<p><strong>Hooks reutilizáveis e genéricos.</strong></p>

<ul>
  <li>useMediaQuery</li>
  <li>useDebounce</li>
  <li>useLocalStorage</li>
  <li>useIsClient</li>
</ul>

<p><strong>Regra:</strong> Hooks com lógica de negócio vão em <code>features/</code>.</p>

<hr />

<h2>📂 lib/</h2>
<p><strong>Infraestrutura global do projeto.</strong></p>

<ul>
  <li>Clientes HTTP (axios/fetch wrapper)</li>
  <li>Configurações globais</li>
  <li>Schemas globais</li>
  <li>Conexões com serviços externos</li>
</ul>

<p><strong>Regra:</strong> Tudo que faz parte do core global do projeto.</p>

<hr />

<h2>📂 services/</h2>
<p><strong>Serviços globais de comunicação externa ou regras centrais do sistema.</strong></p>

<ul>
  <li>Serviço de autenticação</li>
  <li>Serviço de leitura de nota fiscal</li>
  <li>Serviços de IA</li>
  <li>Processamentos e integrações gerais</li>
</ul>

<p><strong>Regra:</strong> Serviços específicos da feature → <code>features/&lt;feature&gt;/services</code>.</p>

<hr />

<h2>📂 styles/</h2>
<p><strong>Estilos globais.</strong></p>

<ul>
  <li>globals.css</li>
  <li>tokens de design</li>
  <li>configurações Tailwind</li>
  <li>animações globais</li>
</ul>

<p><strong>Regra:</strong> Estilos específicos devem ficar dentro da feature.</p>

<hr />

<h2>📂 utils/</h2>
<p><strong>Funções puras e reutilizáveis.</strong></p>

<ul>
  <li>formatadores</li>
  <li>máscaras</li>
  <li>funções matemáticas</li>
  <li>validações simples</li>
  <li>manipulação de datas</li>
</ul>

<p><strong>Regra:</strong> Funções específicas da feature → <code>features/&lt;feature&gt;/utils</code>.</p>

<hr />

<h2>📦 Exemplo de Estrutura Final</h2>

<pre><code>app/
  layout.tsx
  page.tsx

components/
  ui/
    button.tsx
    card.tsx

features/
  shopping-list/
    components/
      shopping-card.tsx
    services/
      shopping-service.ts
    hooks/
      use-shopping.ts
    types/
      shopping-types.ts
    utils/
      shopping-formatter.ts

hooks/
  useDebounce.ts
  useMediaQuery.ts

lib/
  api-client.ts

services/
  auth-service.ts

styles/
  globals.css

utils/
  format-date.ts
  mask-cpf.ts
</code></pre>

<hr />

<h2>🎯 Princípios da Arquitetura</h2>

<ul>
  <li><strong>Baixo acoplamento</strong> — partes independentes.</li>
  <li><strong>Alta coesão</strong> — cada pasta tem uma responsabilidade clara.</li>
  <li><strong>Escalabilidade</strong> — novas features não quebram antigas.</li>
  <li><strong>Previsibilidade</strong> — fácil encontrar qualquer arquivo.</li>
  <li><strong>Modularização</strong> — facilita PRs e reduz conflitos.</li>
</ul>

<hr />

<h2>🎉 Conclusão</h2>
<p>
  A arquitetura proposta garante organização, modularidade e escalabilidade. O sistema pode crescer de forma
  saudável, mantendo previsibilidade e facilidade de manutenção.
</p>
