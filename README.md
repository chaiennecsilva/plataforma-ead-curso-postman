## Workflow Automatizado com GitHub Actions

Este repositório inclui um fluxo de trabalho automatizado utilizando o GitHub Actions. Aqui está um resumo do que ele faz:

### Funcionalidades do Fluxo de Trabalho:

1. **Execução Automática:**
   - O fluxo de trabalho é acionado automaticamente em duas situações:
     - Quando há uma alteração ou push no ramo "main".
     - Quando uma solicitação de pull é aberta para o ramo "main".

2. **Execução Manual:**
   - Você também pode executar manualmente este fluxo de trabalho a partir da guia "Actions" no GitHub.

### Descrição dos Passos:

1. **Verificação de Versões:**
   - O fluxo de trabalho verifica as versões do Newman e do Node.js.

2. **Instalação de Dependências:**
   - Instala o pacote `newman-reporter-htmlextra` globalmente.

3. **Execução da Coleção:**
   - Executa uma coleção de testes utilizando Newman, gerando um relatório HTML extra.
   - O relatório é exportado para `./result/Report.html`.

4. **Arquivamento de Artefatos:**
   - Após a execução, o relatório é arquivado como um artefato do processo.

### Como Usar:

- Certifique-se de que suas alterações estejam no ramo "main".
- Você pode monitorar o progresso e visualizar os resultados na guia "Actions" deste repositório.

Este fluxo de trabalho automatizado ajuda a garantir a integridade e qualidade do código neste projeto.
