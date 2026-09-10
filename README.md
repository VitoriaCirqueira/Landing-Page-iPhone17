# iPhone 17 Pro

Landing page conceitual do iPhone 17 Pro, desenvolvida para fins educacionais durante as aulas do DevClub. O projeto recria uma página de apresentação de produto com foco em composição visual, navegação por seções, responsividade e componentes reutilizáveis.

> Este projeto é um protótipo front-end. Os textos, imagens, especificações e valores são demonstrativos e não representam uma loja oficial da Apple. Os botões de compra e links institucionais ainda não possuem integração com checkout ou backend.

## Visão geral

A página apresenta o produto em uma experiência de rolagem única, com navegação fixa no topo e seções organizadas por assunto:

- **Hero:** imagem principal do produto e indicação visual para continuar a rolagem.
- **Introdução:** título, proposta de valor, chamadas para ação e cards com especificações.
- **Design:** destaques visuais sobre titânio e sistema operacional.
- **Performance:** apresentação conceitual do chip A18 Pro e seus principais números.
- **Câmera:** cards com as características dos sensores.
- **Cores:** seleção interativa entre as opções de acabamento do aparelho.
- **Rodapé:** links organizados por categorias e informações institucionais.

## Tecnologias utilizadas

- **React 19:** construção da interface por componentes e gerenciamento do estado da cor selecionada.
- **Vite:** servidor de desenvolvimento, atualização rápida com HMR e build de produção.
- **JavaScript com JSX:** lógica e marcação da interface em arquivos `.jsx`.
- **Tailwind CSS 4:** estilização utilitária, responsividade, espaçamento, cores, grids, efeitos e transições.
- **CSS global:** reset básico, fonte, rolagem suave, espaço para a navbar fixa e utilitário de texto gradiente.
- **ESLint:** análise estática e validação de boas práticas para JavaScript e React.
- **HTML semântico:** uso de elementos como `nav`, `section`, `button`, `img` e `footer`.

## Funcionalidades

- Navbar fixa com links de navegação por âncoras.
- Rolagem suave entre as seções da página.
- Espaçamento de rolagem para evitar que a navbar cubra os títulos das seções.
- Seleção interativa de cor usando `useState`.
- Atualização da imagem e do nome do acabamento conforme a cor escolhida.
- Layouts com grids e flexbox para diferentes tamanhos de tela.
- Estados visuais de hover, transições e animações com classes do Tailwind.
- Uso de imagens locais para o hero, acabamentos, design e chip.

## Estrutura do projeto

```text
.
├── public/
│   └── img/
│       ├── chip-a18-pro.jpg
│       ├── hero.jpg
│       ├── ios-features.jpg
│       ├── iphone-blue.jpg
│       ├── iphone-orange.jpg
│       ├── iphone-silver.jpg
│       └── titanium-design.jpg
├── src/
│   ├── components/
│   │   ├── Colors.jsx
│   │   ├── Footer.jsx
│   │   ├── Hero.jsx
│   │   ├── Highligths.jsx
│   │   ├── Intro.jsx
│   │   └── NavBar.jsx
│   ├── App.jsx
│   ├── index.css
│   └── main.jsx
├── eslint.config.js
├── index.html
├── package.json
└── vite.config.js
```

### Organização dos componentes

- `main.jsx` inicializa o React e importa o CSS global.
- `App.jsx` define a composição principal da landing page.
- `NavBar.jsx` contém a navegação fixa e os links para as âncoras.
- `Hero.jsx` apresenta a imagem de abertura.
- `Intro.jsx` reúne a mensagem principal, botões e especificações resumidas.
- `Highligths.jsx` concentra as seções de design, performance e câmera.
- `Colors.jsx` controla a escolha de acabamento com `useState`.
- `Footer.jsx` organiza os links finais e as informações institucionais.

## Como executar

### Pré-requisitos

- Node.js instalado.
- npm instalado.

### Instalação

Clone o repositório e instale as dependências:

```bash
git clone https://github.com/VitoriaCirqueira/Landing-Page---iPhone17.git
cd Landing-Page---iPhone17
npm install
```

### Desenvolvimento

Inicie o servidor local:

```bash
npm run dev
```

O Vite exibirá no terminal o endereço local para acessar a aplicação, normalmente `http://localhost:5173`.

### Build de produção

Para gerar os arquivos otimizados:

```bash
npm run build
```

Para visualizar o build localmente:

```bash
npm run preview
```

### Lint

Para verificar problemas de código:

```bash
npm run lint
```

## Aprendizados do projeto

Este projeto foi utilizado para praticar:

- criação de componentes funcionais em React;
- composição de uma página a partir de componentes menores;
- renderização de listas com `map` e uso de `key`;
- gerenciamento de estado com o hook `useState`;
- navegação interna com links e IDs de seção;
- construção de layouts com flexbox e CSS Grid;
- aplicação de breakpoints e classes responsivas do Tailwind;
- organização de dados de apresentação em arrays JavaScript;
- uso de imagens locais em uma aplicação Vite;
- validação do código com ESLint;
- geração de build para produção com Vite.

## Próximos passos

- Conectar os botões de compra a um fluxo real de produto ou checkout.
- Transformar os links do rodapé em rotas ou páginas funcionais.
- Adicionar acessibilidade aprimorada, incluindo `aria-labels` e foco visível nos controles.
- Refinar os breakpoints das grades para telas pequenas.
- Corrigir e padronizar textos e especificações do conteúdo demonstrativo.
- Adicionar testes para a seleção de cores e para a navegação entre seções.

## Licença e finalidade

Projeto criado exclusivamente para estudo e prática de desenvolvimento front-end. Não possui vínculo comercial com a Apple.
