# Tarefa 33 — Página pessoal com DaisyUI

Este projeto foi desenvolvido para a Tarefa 33 da disciplina de Design Web. A proposta foi criar uma página pessoal responsiva utilizando componentes do DaisyUI como base da interface, complementados por classes utilitárias do Tailwind CSS.

## Componentes DaisyUI utilizados

- **navbar** — utilizada no topo da página para apresentar o nome, links de navegação, botão de contato e controle de tema.
- **hero** — utilizada na seção inicial para destacar a apresentação principal.
- **btn** — utilizada nos botões de navegação e ações. Foram usadas variações como `btn-primary`, `btn-outline` e `btn-ghost`.
- **badge** — utilizada para destacar área de atuação, habilidades e categorias dos projetos. Foram usadas variações como `badge-primary`, `badge-secondary` e `badge-outline`.
- **card** — utilizada na seção de projetos e também no formulário de contato. Cada projeto possui `card-body`, `card-title` e `card-actions`.
- **input** — utilizada nos campos de nome e e-mail do formulário.
- **textarea** — utilizada no campo de mensagem.
- **alert** — utilizada para destacar uma informação na seção de contato.
- **theme-controller** — utilizado para permitir a alternância entre os temas claro e escuro.

## Escolha do cabeçalho

Escolhi combinar `navbar` e `hero`.

A `navbar` foi usada porque facilita a navegação entre as principais seções da página e mantém ações importantes sempre acessíveis. Já o `hero` foi utilizado logo abaixo para dar destaque à apresentação pessoal e aos principais botões de ação.

Essa combinação permite separar a navegação da apresentação principal, deixando a estrutura mais organizada.

## Ajustes feitos com Tailwind CSS

Apesar de o DaisyUI fornecer os componentes principais, algumas classes do Tailwind foram utilizadas para ajustar o layout.

### 1. Responsividade da seção de projetos

Foi utilizado:

```html
grid gap-6 md:grid-cols-2 lg:grid-cols-3
```

Isso permite que os cards sejam exibidos em uma coluna em telas pequenas, duas em telas médias e três em telas maiores.

### 2. Espaçamento e largura do conteúdo

Classes como:

```html
max-w-6xl mx-auto px-4 py-20
```

foram utilizadas para limitar a largura máxima do conteúdo, centralizar a página e criar espaçamentos consistentes.

Também foram usadas classes responsivas, como `lg:flex-row`, `md:grid-cols-2` e `hidden md:flex`, para adaptar o layout ao tamanho da tela.

## Temas

A página foi testada com os temas `light` e `dark`.

O tema **dark** ficou especialmente coerente com a proposta de uma página voltada para tecnologia, enquanto o tema **light** oferece uma aparência mais limpa e neutra.

Os componentes utilizam cores semânticas do DaisyUI, como `bg-base-100`, `bg-base-200`, `text-base-content` e `btn-primary`. Por isso, as cores se adaptam automaticamente quando o tema é alterado, mantendo contraste e legibilidade.

## Responsividade

O layout foi planejado para funcionar em diferentes tamanhos de tela.

- No celular, as seções ficam principalmente em uma coluna.
- Em telas médias, alguns conteúdos passam a utilizar duas colunas.
- Em telas maiores, os três projetos aparecem lado a lado.
- Os links centrais da navbar ficam ocultos em telas menores para evitar falta de espaço.

## Estrutura da página

A página possui as seguintes seções:

1. Cabeçalho e navegação
2. Apresentação pessoal
3. Habilidades
4. Projetos
5. Contato
6. Rodapé

O objetivo foi utilizar os componentes do DaisyUI como base da interface e complementar apenas o necessário com classes do Tailwind CSS.
