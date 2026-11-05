# Especificação do Projeto: Página Web Responsiva com Bootstrap 5 e Tailwind CSS

## 1. Instruções ao agente

Este documento é a única fonte de verdade da atividade. Leia-o por completo antes de gerar qualquer artefato.

### 1.1 Escopo

- Siga apenas o que está descrito neste documento, e nada além disso.
- Não adicione componentes, páginas, funcionalidades, bibliotecas ou requisitos que não estejam listados aqui.
- Em caso de dúvida, não presuma. Implemente somente o que está escrito.

### 1.2 Regra sobre comentários no código

O código final não deve possuir comentários de nenhum tipo.

Isso é um requisito da atividade e vale para todos os arquivos gerados: HTML, CSS e JavaScript. Esta regra tem prioridade sobre qualquer outra orientação de estilo.

- Não use comentários de linha (`//`).
- Não use comentários de bloco (`/* ... */`).
- Não use comentários em HTML (`<!-- ... -->`).
- Não use blocos de documentação (JSDoc e similares).
- Não deixe marcações como `TODO`, `FIXME` ou `NOTE`.
- Não deixe código comentado.

Como o código não terá comentários, ele deve ser autoexplicativo:

- Use nomes claros e descritivos para variáveis, funções, classes próprias, ids e arquivos.
- Mantenha as funções pequenas e com uma única responsabilidade.
- Use indentação consistente em todos os arquivos.

Antes de entregar, revise todos os arquivos e remova qualquer comentário que tenha restado.

### 1.3 Ponto de partida e organização dos arquivos

A pasta **`Elton-entrega2`** é o ponto de partida. Crie tudo dentro dela e não crie arquivos fora dela.

A atividade exige duas soluções independentes, reunidas no mesmo pacote:

```
Elton-entrega2/
├── bootstrap/
│   └── index.html
└── tailwind/
    └── index.html
```

Regras da organização:

- Cada solução é independente da outra e deve funcionar sozinha, abrindo o `index.html` da sua pasta no navegador.
- As duas pastas não compartilham nenhum arquivo. Nenhum arquivo de uma pasta pode referenciar arquivos da outra.
- Se uma solução precisar de arquivos além do `index.html` (por exemplo, um arquivo de JavaScript), eles ficam dentro da pasta dela.
- As duas soluções devem ter o mesmo tema, o mesmo conteúdo e os mesmos 6 componentes, para que possam ser comparadas.

## 2. Tema e objetivo

**Objetivo:** desenvolver uma página web responsiva utilizando frameworks CSS modernos.

**Tema:** Reservas de academia na cidade de Salvador, BA.

Todo o conteúdo exibido nos componentes deve ser fictício, mas semanticamente relevante para o tema e para o tipo de componente. Cada componente deve demonstrar funcionalidade clara e propósito bem definido.

## 3. Condições da atividade

Estas condições valem para as duas soluções.

### 3.1 Estrutura da página

A página deve conter uma estrutura básica de HTML5, incluindo:

- `header`
- `main`, com pelo menos uma `section`
- `footer`

### 3.2 Responsividade

- A página deve ser totalmente responsiva, adaptando-se a smartphones, tablets e desktops.
- O layout deve ser fluido e os elementos devem se reorganizar de forma adequada em diferentes resoluções de tela.

### 3.3 Componentes

A página deve incorporar, no mínimo, 6 componentes visuais distintos. Os componentes obrigatórios são:

| Componente | Descrição | Uso no tema |
|---|---|---|
| Navbar | Barra de navegação responsiva com menu colapsável | Menu principal do site |
| Carrossel | Galeria de imagens com navegação | Destaques de academias |
| Cards | Componentes de conteúdo estruturado | Listagem de academias ou serviços |
| Tabela | Apresentação de dados tabulares | Listagem de horários e vagas |
| Formulário | Campos de entrada e envio de dados | Cadastro para reserva ou contato |
| Modal/Diálogo | Janela sobreposta com conteúdo | Confirmação de reserva ou detalhes |

### 3.4 Acessibilidade e semântica

- Usar corretamente tags semânticas do HTML5.
- Usar atributos ARIA quando necessário.

## 4. Especificação por componente

Itens marcados como **(opcional)** podem ser implementados ou não. Se implementar um item opcional, implemente-o nas duas soluções.

### 4.1 Navbar (Barra de Navegação)

Deve incluir:

- Logo ou título do site.
- Menu de navegação com pelo menos 3 itens.
- Menu colapsável (hamburger menu) em dispositivos móveis.
- Estilo visual consistente com o restante da página.

### 4.2 Carrossel (Carousel)

Deve incluir:

- Pelo menos 3 slides com imagens ou conteúdo.
- Botões de navegação (anterior e próximo).
- Indicadores de slide (dots).
- Transição suave entre slides.
- Funcionalidade de auto-play **(opcional)**.

### 4.3 Cards (Componentes de Conteúdo)

Deve incluir:

- Pelo menos 3 cards dispostos em grid responsivo.
- Título e descrição em cada card.
- Reorganização automática em diferentes tamanhos de tela.
- Imagem ou ícone **(opcional)**.
- Botão de ação **(opcional)**.

### 4.4 Tabela (Dados Tabulares)

Deve incluir:

- Cabeçalho com títulos das colunas.
- Pelo menos 5 linhas de dados.
- Estilo visual claro e legível.
- Responsividade, com scroll horizontal em mobile ou reorganização.
- Alternância de cores de linha (striped) para melhor legibilidade.

### 4.5 Formulário (Form)

Deve incluir:

- Pelo menos 4 campos de entrada (text, email, textarea, etc.).
- Labels associados aos campos.
- Botão de envio.
- Validação básica (HTML5).
- Layout responsivo.

### 4.6 Modal/Diálogo (Modal)

Deve incluir:

- Botão para abrir o modal.
- Conteúdo modal com título e descrição.
- Botões de ação (fechar, confirmar, etc.).
- Sobreposição (overlay) semi-transparente.
- Fechar ao clicar fora **(opcional)**.

## 5. Solução 1: Bootstrap 5

Pasta: `Elton-entrega2/bootstrap/`

- A solução principal deve ser desenvolvida utilizando o framework **Bootstrap 5**.
- A integração do Bootstrap deve ser feita via CDN, incluindo o CSS e o JavaScript do Bootstrap.
- Use as classes e os componentes nativos do Bootstrap para garantir a responsividade e o estilo.
- Todos os 6 componentes devem ser implementados utilizando os componentes e as classes do Bootstrap.

## 6. Solução 2: Tailwind CSS (desafio extra)

Pasta: `Elton-entrega2/tailwind/`

Esta solução vale 0,2 ponto adicional e deve ser independente da solução com Bootstrap.

- Utilize as classes utilitárias do Tailwind CSS para estilização e responsividade.
- A integração do Tailwind CSS deve ser feita via CDN.
- Todos os 6 componentes devem estar presentes e funcionais.
- A solução deve demonstrar compreensão da abordagem **utility-first** do Tailwind: a estilização fica nas classes utilitárias aplicadas diretamente nos elementos.
- Como o Tailwind não traz componentes interativos prontos, o comportamento dos componentes (menu colapsável, carrossel e modal) deve ser feito com JavaScript nativo.

## 7. Restrições

- **Dependências:** utilize apenas o framework CSS especificado em cada solução (Bootstrap ou Tailwind) e JavaScript nativo quando necessário. Não adicione outras bibliotecas ou frameworks.
- **Código limpo:** indentação consistente e nomes descritivos. Sem comentários, conforme a seção 1.2.

## 8. Observações da atividade (para a pessoa, não para o agente)

- O trabalho é estritamente individual.
- **Vídeo obrigatório:** gravar e enviar um vídeo curto explicando a solução desenvolvida, demonstrando o funcionamento dos componentes e passando pelo código implementado.
- **Vídeo do desafio extra:** gravar um novo vídeo apresentando a solução com Tailwind CSS e comparando-a com a solução em Bootstrap.
- **Ambiente obrigatório:** GitHub Codespaces.
- **Testes de responsividade:** testar a aplicação em mobile, tablet e desktop.
- **Testes em navegadores:** testar todos os componentes no Chrome, Firefox, Safari e Edge.

## 9. Checklist de entrega

- [ ] Tudo foi criado dentro da pasta `Elton-entrega2`, em duas pastas independentes: `bootstrap` e `tailwind`.
- [ ] Nenhum arquivo de uma solução depende de arquivos da outra.
- [ ] Apenas o que consta neste documento foi implementado.
- [ ] As duas soluções têm `header`, `main` (com pelo menos uma `section`) e `footer`.
- [ ] Os 6 componentes estão presentes e funcionais nas duas soluções: Navbar, Carrossel, Cards, Tabela, Formulário e Modal.
- [ ] Cada componente segue as regras da seção 4 e usa conteúdo fictício do tema.
- [ ] A solução Bootstrap usa Bootstrap 5 via CDN, com classes e componentes nativos.
- [ ] A solução Tailwind usa Tailwind CSS via CDN, com classes utilitárias, e JavaScript nativo para o comportamento.
- [ ] Tags semânticas do HTML5 e atributos ARIA estão aplicados.
- [ ] O layout é responsivo em mobile, tablet e desktop.
- [ ] Nenhuma biblioteca além do framework CSS de cada solução foi adicionada.
- [ ] Nenhum arquivo de código contém comentários de qualquer tipo.