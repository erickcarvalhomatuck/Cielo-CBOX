# Center Box - Analisador de Extratos Cielo

**Center Box** é uma ferramenta web gratuita e de código aberto desenvolvida para simplificar e automatizar a análise de extratos financeiros da Cielo. O sistema transforma o processo manual de cálculo em planilhas em uma experiência rápida e intuitiva, gerando relatórios gerenciais (PDF) com as informações essenciais para o seu dia a dia.

## Motivação

A Cielo não oferece uma forma simples de exportar um extrato resumido com os valores líquidos por bandeira. Analistas e contadores frequentemente precisam baixar o extrato completo e realizar cálculos manuais no Excel, um processo demorado, repetitivo e sujeito a erros. Este sistema foi criado para automatizar essa tarefa, permitindo que você foque no que realmente importa: a análise dos resultados.

## Funcionalidades

*   **Upload Inteligente:** Carrega o arquivo Excel (.xlsx, .xls) do extrato da Cielo.
*   **Processamento Automático:** Identifica automaticamente as colunas necessárias (`Bandeira`, `Valor Líquido`, `Data do Lançamento`, `Tipo de lançamento`) e processa os dados.
*   **Extrato Complementar/Técnico (Relatório Essencial):** Gera um resumo executivo com:
    *   **CPF/CNPJ** do estabelecimento.
    *   **Data de Pagamento** do extrato.
    *   **Total e detalhamento por bandeira** para vendas Crédito e Débito.
    *   **Download em PDF** para arquivamento ou envio.
*   **Extrato Detalhado:** Apresenta uma visão aprofundada dos lançamentos, permitindo:
    *   **Filtrar** os resultados por "Crédito", "Débito" ou "Todos".
    *   Visualizar o **valor líquido total** e o **detalhamento por data** para cada bandeira.
    *   **Download em PDF** para análises mais completas.
*   **Identificação de Matriz/Filiais:** O sistema captura o **CPF/CNPJ** do extrato, facilitando a diferenciação de relatórios para empresas com múltiplas filiais.
*   **Interface Amigável:** Design clean e responsivo, com um tutorial integrado para guiar o usuário no primeiro uso.

## Como Usar

1.  **Acesse a ferramenta:** Abra o arquivo `CENTER BOX - CIELO 4.0.html` no seu navegador de internet preferido (Chrome, Edge, Firefox).
2.  **Carregue o extrato:** Clique no botão "Carregar Arquivo" e selecione o arquivo Excel (.xlsx ou .xls) baixado do sistema da Cielo.
3.  **Processe os dados:** Clique em "Processar Arquivo". O sistema fará toda a análise automaticamente.
4.  **Analise os resultados:**
    *   O **"Extrato Complementar/Técnico"** será exibido com o resumo essencial. Clique em "Gerar PDF Técnico" para salvá-lo.
    *   Role a página até **"Resultados Detalhados"**. Use o filtro para alternar entre Crédito e Débito. Clique em "Gerar PDF Detalhado" para obter o relatório completo.

## Tecnologias Utilizadas

*   **HTML5:** Estrutura da página.
*   **CSS3:** Estilização e design responsivo.
*   **JavaScript (ES6+):** Toda a lógica de processamento e interação.
*   **[SheetJS (xlsx)](https://cdnjs.com/libraries/xlsx):** Biblioteca para leitura e parsing de arquivos Excel.
*   **[jsPDF](https://cdnjs.com/libraries/jspdf) & [jsPDF-AutoTable](https://cdnjs.com/libraries/jspdf-autotable):** Bibliotecas para geração dos relatórios em PDF.

## Requisitos do Arquivo de Entrada

Para que o sistema funcione corretamente, o arquivo Excel deve ser o extrato padrão gerado pela Cielo e conter as seguintes colunas:

*   `Bandeira`
*   `Valor Líquido`
*   `Data do Lançamento`
*   `Tipo de lançamento` (com os valores "Venda crédito" e "Venda débito")

> **Dica:** Quanto mais fiel ao formato original do extrato, melhor o sistema conseguirá identificar e processar os dados.
> Vales ainda não estão sendo identificados pelo extrato, não foram implementados nessa versão, virá em versão futura.

## Como Contribuir

Contribuições são sempre bem-vindas! Se você tem uma ideia, encontrou um bug ou quer melhorar o código, sinta-se à vontade para:

1.  Fazer um **fork** do projeto.
2.  Criar uma **branch** para sua feature (`git checkout -b feature/nova-feature`).
3.  Fazer **commit** das suas alterações (`git commit -m 'Adiciona nova feature'`).
4.  Fazer **push** para a branch (`git push origin feature/nova-feature`).
5.  Abrir um **Pull Request**.

## Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---
**Center Box** - Simplificando a análise de recebíveis Cielo.
