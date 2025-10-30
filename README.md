🪄 Magic Banner Plugin — Desafio Técnico Futuriza
=================================================

🚀 Descrição do Desafio
-----------------------

Este repositório contém o desafio técnico **"Magic Banner Plugin"**, proposto pela **Futuriza**.O objetivo é desenvolver uma aplicação **Next.js full stack** que permita criar e exibir **banners personalizados** em páginas de e-commerce, com base na **URL atual do site** e, opcionalmente, no **horário de exibição**.

A ideia é que qualquer loja possa exibir banners dinâmicos apenas **importando um script**.

🧱 Requisitos do Projeto
------------------------

### 🔹 Funcionalidades obrigatórias

*   Painel administrativo para **criar, listar e excluir banners**.
    
*   Cada banner deve conter:
    
    *   **URL completa** da página de destino (ex: https://lojaexemplo.com/produto/123)
        
    *   **Imagem do banner** (upload ou link)
        
    *   **Horário de exibição (opcional)** — ex: das 08:00 às 12:00
        
*   **API de banners** que recebe uma URL e retorna o banner correspondente.
    
*   **Script embutível** (/public/magic-banner.js) que:
    
    *   Captura a URL da página.
        
    *   Faz uma requisição para /api/banners?url=.
        
    *   Exibe o banner dinamicamente no topo da página.
        

### 🔹 Requisitos técnicos

*   **Next.js 14+**
    
*   **API Routes** para backend
    
*   **Persistência** (Supabase, SQLite ou JSON local)
    
*   **Deploy na Vercel (conta gratuita)**
    

🖥️ Estrutura esperada
----------------------

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   .  ├── app/ ou pages/          # Rotas e views (Next.js)  ├── pages/api/banners.js    # API dos banners  ├── public/magic-banner.js  # Script embutível  ├── /lib ou /db             # Persistência ou conexão  └── README.md               # Documentação   `

⚙️ Como rodar o projeto localmente
----------------------------------

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   # 1. Clone este repositório  git clone https://github.com//magic-banner-futuriza.git  # 2. Acesse a pasta  cd magic-banner-futuriza  # 3. Instale as dependências  npm install  # 4. Rode o servidor de desenvolvimento  npm run dev   `

> O projeto estará disponível em: http://localhost:3000

🧩 Como testar o script embutível
---------------------------------

1.  Faça o deploy do projeto na **Vercel**.
    
2.  Em qualquer página HTML, adicione a tag abaixo:
    

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`  `

1.  Ao carregar a página, o script fará uma requisição para:
    

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   https://.vercel.app/api/banners?url=   `

Se houver um banner cadastrado para aquela URL, ele será exibido automaticamente no topo do site.

🪄 Exemplo de funcionamento
---------------------------

*   Banner cadastrado para:https://lojaexemplo.com/produto/123
    
*   Quando o script é carregado nessa URL, ele exibe o banner dinamicamente.
    
*   Se o horário de exibição estiver definido, o banner só aparece dentro do intervalo configurado.
    

🧠 Decisões técnicas (preencher pelo candidato)
-----------------------------------------------

Descreva aqui as principais decisões tomadas durante o desenvolvimento, por exemplo:

*   Frameworks e bibliotecas utilizadas
    
*   Estratégia de persistência
    
*   Estrutura de pastas e componentes
    
*   Como foi feita a lógica de exibição condicional dos banners
    
*   Desafios encontrados e como foram resolvidos
    

🌟 Diferenciais implementados (opcional)
----------------------------------------

Liste aqui os diferenciais adicionados, como:

*   Upload real de imagem (Supabase Storage)
    
*   Autenticação no painel
    
*   Efeitos visuais no banner
    
*   Preview em tempo real
    

🔗 Deploy
---------

*   **Painel administrativo:** https://.vercel.app/admin
    
*   **Script público:** https://.vercel.app/magic-banner.js
    

📅 Prazo de entrega
-------------------

**7 dias corridos** após o envio do desafio.

Entregar:

*   Link do repositório público (GitHub)
    
*   Link do deploy na Vercel
    
*   (Opcional) GIF ou vídeo curto mostrando o funcionamento
    

🧪 Critérios de avaliação
-------------------------

CritérioDescrição**Organização de código**Estrutura clara, componentes bem definidos e boas práticas.**Integração full stack**Comunicação fluida entre painel, API e script embutível.**Domínio de Next.js**Uso correto de rotas, APIs, SSR/ISR e deploy.**Funcionalidade real**Banner aparecendo dinamicamente conforme a URL.**UX/UI**Painel funcional e usabilidade simples.**Documentação e Deploy**Facilidade de entendimento e reprodução.

💡 Sobre a Futuriza
-------------------

A **Futuriza** é uma empresa de tecnologia focada em **acelerar o futuro do varejo**, desenvolvendo soluções inteligentes com **IA, automação e geração de imagens**.Entre seus produtos estão **plugins inteligentes para e-commerce**, como **video commerce**, **provador virtual com IA** e **sugestão de tamanho automatizada**.

🧩 **Boa sorte!**Capriche na clareza do código, na organização e na experiência do painel.Queremos ver como você estrutura uma aplicação real de ponta a ponta 🚀
