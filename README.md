# SpinRide

Landing page para uma loja fictícia de bicicletas.

## Sobre o Projeto

Criado como projeto final da disciplina _Desenvolvimento de Interfaces Web com HTML5 e CSS3_ da Pós-graduação em Web pela UTFPR.

#### 1. Estrutura Semântica Rigorosa: Construir o layout completo utilizando apenas tags semânticas (Módulo 01), garantindo que a estrutura seja compreensível para motores de busca e leitores de tela.

O layout foi estruturado com as tags semânticas do HTML5: `<header>` para o cabeçalho com navegação, `<section>` para delimitar as áreas de conteúdo (hero e serviços), `<footer>` para o rodapé, `<ul>` e `<li>` para listas de links e cards de serviço, e hierarquia de títulos (`h1` → `h5`) respeitando a ordem lógica do documento. O atributo `alt` foi aplicado em todas as imagens e o atributo `lang="pt-br"` foi definido na tag `<html>`, favorecendo acessibilidade e leitura por motores de busca.

#### 2. Sistema de Design com Variáveis: Implementar um esquema de cores e tipografia centralizado em variáveis CSS, permitindo a troca de identidade visual do seu tema de forma global e organizada (Módulo 02).

As variáveis CSS foram declaradas no seletor `:root`, centralizando toda a identidade visual do projeto. As cores principais (`--primary-color: #FF5C00`, `--secondary-color: #1b3022`, `--muted-color`, `--text-white` e `--text-muted`) e as duas famílias tipográficas (*Hanken Grotesk* e *Montserrat*, importadas via Google Fonts) são referenciadas em todo o stylesheet via `var()`, de modo que qualquer alteração de tema exige mudança em um único lugar.

#### 3. Layout Híbrido (Flex & Grid): Criar seções que combinem o alinhamento do Flexbox (menus/botões) com a robustez do CSS Grid para o posicionamento da grade principal de conteúdo (Módulo 03).

O posicionamento foi construído inteiramente com Flexbox: `display: flex` com `flex-direction: column` é usado no mobile para empilhar o header, seções e cards de serviço, e alterado para `flex-direction: row` via media query (`min-width: 768px`) para alinhar os itens lado a lado no desktop. CSS Grid não chegou a ser utilizado nesta versão do projeto.

#### 4. Interface Responsiva: Garantir que o projeto seja adequado para telas pequenas (mobile) e escale com fluidez até resoluções desktop, sem quebras visuais (Módulo 04).

A abordagem adotada foi *mobile-first*: o layout base foi projetado para telas pequenas e adaptado em dois breakpoints via `@media`. Em `min-width: 768px`, a navegação é exibida, os botões do hero passam para linha horizontal, os cards de serviço se reorganizam em linha e o footer muda para layout horizontal. Em `min-width: 1024px`, o título do hero e as colunas do footer são reajustados para melhor aproveitamento em telas maiores.

#### 5. Microinterações de Feedback: Desenvolver animações de entrada e estados de hover que deem vida à interface e melhorem a experiência do usuário (Módulo 05).

Curadoria de Código com IA: Utilizar IA para gerar e refatorar um componente específico da sua página, documentando como você validou e ajustou o código gerado para o seu projeto (Módulo 06).

Implementação de Dark Mode Nativo (Pesquisa): Pesquisar e aplicar a media query prefers-color-scheme para que o seu site se adapte automaticamente às preferências de tema do sistema do usuário.

Sticky Headers e Scroll Snap (Pesquisa): Pesquisar propriedades de scroll do CSS para criar um cabeçalho fixo e seções que se ajustam suavemente à tela durante a navegação.

Otimização de Performance e Assets (Pesquisa): Pesquisar sobre formatos de imagem modernos (como WebP) e carregamento de fontes para garantir que sua landing page abra instantaneamente. Tente atingir uma pontuação de performance próxima de 100 no Google PageSpeed.

Acessibilidade Avançada com Teclado (Pesquisa): Pesquisar e implementar o gerenciamento de foco visual (:focus-visible) e atributos ARIA básicos para garantir que qualquer pessoa consiga navegar no seu projeto sem usar o mouse.
