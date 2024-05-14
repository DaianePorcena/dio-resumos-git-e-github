# Commits Semânticos

Commits semânticos são uma convenção para estruturar mensagens de commit de forma padronizada e significativa. O objetivo é tornar mais fácil entender o propósito e o impacto das mudanças feitas em um projeto de software ao analisar seu histórico de commits. Essa convenção fornece uma estrutura clara para documentar alterações, tornando mais simples para os desenvolvedores colaborarem e acompanharem a evolução do projeto.

## Por que Usar Commits Semânticos?

Commits semânticos oferecem várias vantagens:

- **Clareza:** Cada mensagem de commit segue um formato consistente, tornando fácil entender a natureza das mudanças em um relance.
- **Brevidade:** Commits semânticos incentivam mensagens concisas, transmitindo informações essenciais sem verbosidade desnecessária.
- **Facilidade de Busca:** Ao aderir a um formato padronizado, os commits se tornam mais pesquisáveis, auxiliando na solução de problemas, revisão de código e análise histórica.
- **Automação:** Ferramentas e scripts podem ser desenvolvidos para analisar automaticamente mensagens de commit, possibilitando tarefas como geração de notas de lançamento, changelogs ou acionamento de pipelines de CI/CD com base no tipo de commit.

## Tipos de Commits
| Tipo |	Descrição|
|------|-----------|
| `feat` | Introduz uma nova funcionalidade ao código. |
| ``fix``	| Corrige um bug no código.
| ``docs`` |	Adiciona ou atualiza documentação. |
| ``style``	| Alterações que não afetam o significado do código (espaços em branco, formatação, etc). |
| ``refactor``	| Refatoração do código sem alterar funcionalidades.|
| ``perf`` |	Melhorias de performance. |
| ``test``	| Adiciona ou corrige testes. |
| ``build``	| Alterações que afetam o sistema de build ou dependências externas (npm, gulp, etc). |
| ``ci``	| Alterações em arquivos e scripts de configuração de CI (Continuous Integration). |
| ``chore``	| Outras mudanças que não modificam arquivos de produção ou testes. |
| ``revert``	| Reverte um commit anterior. |