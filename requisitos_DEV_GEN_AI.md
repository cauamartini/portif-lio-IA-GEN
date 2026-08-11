# Documento de Requisitos — DEV_GEN_AI

## 1. Visão geral

O projeto é uma página web/portfólio em português (`pt-BR`) dedicada à apresentação de um curso de **IA Generativa aplicada à Programação**. A página apresenta informações do curso, conhecimentos adquiridos, tecnologias, projetos desenvolvidos, certificação e links externos.

A implementação observada está concentrada em um único arquivo HTML, utilizando Tailwind CSS via CDN, Google Fonts e Material Symbols. Não foram identificados arquivos JavaScript ou backend no material analisado. fileciteturn0file0

## 2. Objetivo

O sistema deve funcionar como uma página institucional/portfólio capaz de:

- Apresentar o curso e sua proposta.
- Exibir informações de carga horária e instituição.
- Apresentar a evolução dos conteúdos estudados.
- Demonstrar conhecimentos técnicos.
- Exibir projetos desenvolvidos.
- Apresentar uma área de certificação.
- Disponibilizar navegação por âncoras entre as seções.
- Disponibilizar links para contato, GitHub, LinkedIn e outras fontes.

## 3. Escopo identificado

### Dentro do escopo

- Interface responsiva.
- Navegação superior fixa.
- Seção inicial/hero.
- Seção de apresentação do curso.
- Linha de evolução de aprendizagem.
- Seção de conhecimentos.
- Seção de projetos.
- Seção de certificação.
- Rodapé institucional.
- Elementos visuais com estética tecnológica.
- Uso de componentes visuais do Material Symbols.
- Uso de Tailwind CSS.
- Uso das fontes Inter e JetBrains Mono.

### Fora do escopo identificado

O HTML não apresenta implementação de:

- Backend.
- Banco de dados.
- Autenticação.
- Cadastro de usuários.
- Persistência de dados.
- APIs funcionais no próprio documento.
- Lógica JavaScript de negócio.
- Sistema real de emissão/validação de certificados.
- Sistema funcional de contato.
- Implementação funcional dos links dos projetos.

Esses itens não devem ser considerados requisitos implementados sem evidências adicionais.

## 4. Principais funções do projeto

Como o arquivo não possui classes ou funções JavaScript declaradas, as “funções” abaixo representam funcionalidades da interface identificadas no HTML.

### RF-01 — Exibir página inicial

O sistema deve apresentar uma seção inicial contendo:

- Nome/identificação `DEV_GEN_AI`.
- Título “IA Generativa aplicada à Programação”.
- Identificação do SENAI Ary Torres, carga horária de 48h e professor.
- Indicação de uso do ChatGPT.
- Texto introdutório.
- Ação para conhecer o curso.
- Ação para visualizar projetos.
- Área visual de perfil do desenvolvedor.

### RF-02 — Navegar pelas seções

O sistema deve disponibilizar navegação por links internos para:

- Home.
- Knowledge.
- Stack.
- Projects.
- Journey.
- Connect.

Os links utilizam âncoras HTML, como `#hero`, `#sobre`, `#projetos` e `#contato`. A seção `contato` não foi identificada no HTML fornecido, portanto esse destino deverá ser revisado. fileciteturn0file0

### RF-03 — Apresentar dados do curso

A página deve apresentar:

- Carga horária: 48h.
- Instituição: SENAI.
- Foco principal: GenAI.
- Área prática: desenvolvimento/programação.

### RF-04 — Apresentar evolução do aprendizado

O sistema deve exibir uma sequência de aprendizagem composta por:

1. Conceitos.
2. Programação.
3. IA.
4. Projetos.
5. APIs.
6. Chatbots.

### RF-05 — Apresentar fluxo de desenvolvimento com IA

A interface deve representar o fluxo:

`IDE → PROMPT → IA → CÓDIGO → TESTE → APLICAÇÃO`

Esse fluxo comunica o uso de IA como apoio ao processo de desenvolvimento.

### RF-06 — Apresentar conhecimentos adquiridos

A página deve apresentar os seguintes conhecimentos:

- IA Generativa e ChatGPT.
- Python.
- Java + IA.
- HTML/CSS/JS.
- APIs.
- Chatbots.
- Machine Learning.
- GitHub e versionamento.

O HTML apresenta indicadores visuais de nível para Python e Java + IA, respectivamente 80% e 70%. Esses valores devem ser tratados como indicadores visuais do portfólio, não como métricas técnicas validadas. fileciteturn0file0

### RF-07 — Exibir projetos

O sistema deve apresentar quatro projetos:

#### Projeto 1 — Jogo Web Interativo

Tecnologias/recursos:

- HTML/JS.
- ChatGPT.

Descrição: jogo para navegador utilizando prompts estruturados para geração de lógica JavaScript e estilização CSS.

#### Projeto 2 — Aplicação Java com IA

Tecnologias/recursos:

- Java.
- Conceitos base de Machine Learning.

Descrição: sistema backend em Java com lógica de tomada de decisão baseada em conceitos de IA.

#### Projeto 3 — Assistente Virtual (Chatbot)

Tecnologias/recursos:

- Python.
- NLP.

Descrição: agente conversacional capaz de interpretar intenções e produzir respostas contextuais dinâmicas.

#### Projeto 4 — Integração Multi-API

Tecnologias/recursos:

- REST APIs.
- OpenAI API.

Descrição: aplicação web conectando serviços externos e processando dados em tempo real com auxílio de GenAI.

As descrições acima são derivadas diretamente do conteúdo dos cards de projetos presentes no HTML. fileciteturn0file0

### RF-08 — Exibir certificação

A página deve disponibilizar uma seção de certificação SENAI contendo:

- Identificação da conclusão do curso.
- Informação de 48 horas de imersão.
- Botão “Visualizar Certificado”.

O HTML apresenta o botão, mas não apresenta uma implementação de abertura, download ou validação do certificado. fileciteturn0file0

### RF-09 — Exibir rodapé

O rodapé deve apresentar:

- Copyright.
- Indicador de sistema online.
- GitHub.
- LinkedIn.
- Source.

Os destinos desses links estão definidos como `#` no HTML fornecido e, portanto, ainda não estão configurados. fileciteturn0file0

## 5. Principais classes/componentes

Não existem classes de programação orientada a objetos declaradas no arquivo. A implementação utiliza principalmente **classes utilitárias CSS do Tailwind** e classes CSS próprias.

### 5.1 Componentes funcionais identificados

| Componente | Responsabilidade |
|---|---|
| Top Navigation | Navegação entre seções |
| Hero | Apresentação principal |
| Developer Profile | Apresentação do aluno/desenvolvedor |
| Course Overview | Resumo do curso |
| Evolution Path | Fluxo de evolução do aprendizado |
| AI Development Flow | Representação do processo com IA |
| Knowledge Base | Apresentação das competências |
| Project Card | Apresentação individual de projeto |
| Certification Card | Apresentação da certificação |
| Footer | Informações institucionais e links |

### 5.2 Classes CSS próprias

#### `.glass-panel`

Responsável pelo efeito visual de painel translúcido, com fundo semitransparente, blur e borda.

#### `.neon-glow-primary`

Responsável pelo efeito de destaque verde ao passar o mouse sobre elementos.

#### `.neon-glow-secondary`

Responsável pelo efeito de destaque ciano ao passar o mouse.

#### `.terminal-bg`

Define fundo escuro para elementos com estética de terminal.

#### `.bg-grid-pattern`

Cria o padrão de grade utilizado como elemento visual da página.

Essas classes são declaradas no bloco `<style>` do HTML. fileciteturn0file0

## 6. Tecnologias identificadas

### Front-end

- HTML5.
- Tailwind CSS via CDN.
- CSS customizado.
- Material Symbols.
- Google Fonts.

### Fontes

- Inter.
- JetBrains Mono.

### Conceitos técnicos apresentados

- JavaScript.
- Python.
- Java.
- HTML.
- CSS.
- REST APIs.
- OpenAI API.
- NLP.
- Machine Learning.
- GitHub.
- ChatGPT.
- IA Generativa.

Essas tecnologias aparecem como conteúdo e/ou recursos visuais da página; sua implementação funcional não é demonstrada pelo único HTML fornecido. fileciteturn0file0

## 7. Requisitos não funcionais

### RNF-01 — Responsividade

A interface deve adaptar sua apresentação para dispositivos móveis e desktop. O HTML utiliza classes responsivas do Tailwind, como `md:grid-cols-2`, `md:flex`, `md:hidden` e outras. fileciteturn0file0

### RNF-02 — Usabilidade

A navegação deve permitir acesso rápido às principais áreas por meio do menu superior e links internos.

### RNF-03 — Identidade visual

A interface deve manter estética tecnológica baseada em:

- Fundo escuro.
- Verde neon.
- Ciano.
- Painéis translúcidos.
- Elementos de terminal.
- Tipografia monoespaçada em elementos técnicos.
- Efeitos de glow.

### RNF-04 — Rolagem suave

O documento HTML utiliza `scroll-smooth` no elemento `<html>`, indicando intenção de navegação com rolagem suave. fileciteturn0file0

### RNF-05 — Desempenho

A página deve carregar os recursos externos utilizados pelo layout, incluindo Tailwind CSS, Google Fonts, Material Symbols e imagens remotas.

## 8. Conteúdo e regras de apresentação

### Regra 01

O nome `DEV_GEN_AI` deve ser apresentado como identificação principal da página.

### Regra 02

A página deve destacar “IA Generativa aplicada à Programação” como tema central.

### Regra 03

A estética visual deve reforçar a relação entre programação, IA e tecnologia.

### Regra 04

Projetos devem apresentar pelo menos:

- Nome.
- Descrição.
- Tecnologias.
- Ação “Ver Projeto”.

### Regra 05

O perfil do desenvolvedor contém conteúdo editável por `contenteditable="true"` no nome/perfil e nos títulos e descrições dos projetos. Isso indica uma possibilidade de edição direta no navegador, mas não existe persistência implementada no HTML. fileciteturn0file0

## 9. Estrutura de navegação

A estrutura principal identificada é:

```text
DEV_GEN_AI
├── Home
│   └── Hero
├── Knowledge
│   ├── Curso
│   ├── Evolution Path
│   └── Knowledge Base
├── Stack
│   └── Conteúdos técnicos
├── Projects
│   ├── Jogo Web Interativo
│   ├── Aplicação Java com IA
│   ├── Assistente Virtual
│   └── Integração Multi-API
├── Journey
│   └── Conteúdo relacionado ao percurso
├── Certificação
└── Footer
    ├── GitHub
    ├── LinkedIn
    └── Source
```

Observação: alguns itens do menu (`Stack`, `Journey` e `Connect`) não possuem seções HTML correspondentes com esses respectivos IDs no arquivo fornecido. fileciteturn0file0

## 10. Fluxo principal do usuário

1. Usuário acessa a página.
2. Visualiza a apresentação do curso.
3. Pode navegar para o conteúdo do curso.
4. Visualiza a evolução de aprendizagem.
5. Consulta os conhecimentos adquiridos.
6. Consulta os projetos desenvolvidos.
7. Pode selecionar “Ver Projeto”.
8. Consulta a certificação.
9. Pode acessar os links do rodapé.

Os links de projeto e rodapé ainda utilizam `href="#"`, portanto o fluxo de navegação externa não está implementado no material analisado. fileciteturn0file0

## 11. Dependências externas

O documento depende de recursos externos:

- Tailwind CSS CDN.
- Google Fonts.
- Material Symbols.
- Imagens hospedadas em `lh3.googleusercontent.com`.

A indisponibilidade desses recursos poderá afetar a aparência ou carregamento de parte da interface. fileciteturn0file0

## 12. Pontos de atenção / pendências

1. Implementar ou corrigir os destinos dos links `href="#"`.
2. Criar a seção `#contato` ou alterar o link “Connect”.
3. Criar as seções correspondentes a `#stack` e `#jornada`, caso façam parte do escopo.
4. Implementar comportamento real do menu mobile.
5. Implementar a ação “Visualizar Certificado”.
6. Definir os URLs reais dos projetos.
7. Definir os URLs reais de GitHub, LinkedIn e Source.
8. Avaliar a necessidade de JavaScript para interações.
9. Avaliar persistência dos campos `contenteditable`.
10. Validar dependências externas para ambiente de produção.
11. Avaliar acessibilidade dos elementos interativos.
12. Substituir placeholders, como “Nome do Aluno”, pelos dados definitivos.

## 13. Critérios de aceite principais

- A página deve abrir corretamente em navegador moderno.
- O menu deve permitir navegar para as seções existentes.
- A página deve funcionar em desktop e dispositivos móveis.
- O curso deve apresentar carga horária de 48h e instituição SENAI.
- Os seis estágios da evolução devem ser apresentados.
- Os oito conhecimentos principais devem estar visíveis.
- Os quatro projetos devem ser apresentados.
- A certificação deve ser exibida.
- Os links externos devem possuir destinos válidos quando forem disponibilizados.
- Elementos atualmente definidos como placeholders devem ser substituídos antes da publicação.

## 14. Resumo técnico

O projeto analisado é essencialmente um **portfolio web estático**, construído em HTML com Tailwind CSS e CSS customizado. Seu principal objetivo é apresentar uma experiência visual de portfólio relacionada a IA Generativa e programação.

Não foram encontradas classes JavaScript, funções JavaScript, componentes de framework ou backend no arquivo analisado. Portanto, requisitos relacionados a processamento, persistência, autenticação ou integração real com APIs precisam de especificação adicional antes de serem considerados implementados.

## 15. Matriz resumida de requisitos

| ID | Requisito | Status observado |
|---|---|---|
| RF-01 | Exibir página inicial | Implementado no HTML |
| RF-02 | Navegação interna | Parcial |
| RF-03 | Exibir dados do curso | Implementado |
| RF-04 | Exibir evolução | Implementado |
| RF-05 | Exibir fluxo IA/desenvolvimento | Implementado |
| RF-06 | Exibir conhecimentos | Implementado |
| RF-07 | Exibir projetos | Implementado visualmente |
| RF-08 | Exibir certificação | Implementado visualmente |
| RF-09 | Exibir rodapé | Implementado |
| RNF-01 | Responsividade | Implementada via Tailwind |
| RNF-02 | Usabilidade | Parcialmente implementada |
| RNF-03 | Identidade visual | Implementada |
| RNF-04 | Rolagem suave | Indicada no HTML |
| RNF-05 | Dependências externas | Implementadas via CDN/URLs |

## 16. Conclusão

O HTML fornece uma base de **portfolio institucional/educacional estático**, com forte foco visual e apresentação de conhecimentos em IA Generativa aplicada à programação.

As principais funcionalidades já representadas são apresentação do curso, navegação, conhecimentos, fluxo de aprendizagem, projetos e certificação. Entretanto, a análise não encontrou lógica de aplicação suficiente para caracterizar o projeto como um sistema funcional completo.

Para uma próxima versão do documento de requisitos, seria necessário analisar também arquivos JavaScript, backend, APIs, banco de dados ou demais arquivos do projeto, caso existam.
