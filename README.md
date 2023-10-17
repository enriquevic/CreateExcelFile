# Classe CreateExcelFile

Este código Java é um utilitário para lidar com arquivos Excel (.xlsx). Ele fornece um método chamado `createExcelFile` que cria ou atualiza um arquivo Excel com base nos parâmetros fornecidos. Aqui está uma explicação passo a passo do que o código faz:

1. **Importação de Bibliotecas:**
   - Importa classes necessárias do Apache POI, uma biblioteca popular para trabalhar com arquivos do Microsoft Office.

2. **Definição da Classe:**
   - Define a classe `ExcelFileHandler`.

3. **Constante de Extensão do Excel:**
   - Declara uma constante que representa a extensão do arquivo Excel.

4. **Método `createExcelFile`:**
   - Assinatura: `public static void createExcelFile(String directory, String fileName, String sheetName, String[][] cellData)`.
   - Cria ou atualiza um arquivo Excel no diretório especificado.
   - Parâmetros:
      - `directory`: O diretório onde o arquivo Excel será armazenado.
      - `fileName`: O nome do arquivo Excel (sem extensão).
      - `sheetName`: O nome da planilha dentro do arquivo Excel.
      - `cellData`: Matriz de dados a serem colocados na planilha.
   - O método tem uma série de mensagens de console (`System.out.printf`) que fornecem feedback sobre o processo.

5. **Array de Mensagens de Texto:**
   - Define um array de strings que contém mensagens formatadas para feedback durante a execução.

6. **Correção do Caminho do Diretório:**
   - Garante que o caminho do diretório termina com uma barra ("/").

7. **Manipulação do Nome do Arquivo e Caminho do Excel:**
   - Adiciona a extensão `.xlsx` ao nome do arquivo e cria um objeto `Path` representando o caminho do arquivo Excel.

8. **Verificação da Existência do Arquivo Excel:**
   - Verifica se o arquivo Excel já existe no diretório especificado.
   - Se não existir, cria um novo arquivo.

9. **Criação do Arquivo Excel e Planilha:**
   - Cria um novo arquivo Excel e uma planilha dentro dele usando a biblioteca Apache POI.
   - Adiciona dados à planilha, se fornecidos.

10. **Verificação do Nome da Planilha:**
    - Se nenhum nome for fornecido para a planilha, ela é chamada de "Planilha".

11. **Adição de Dados à Planilha:**
    - Adiciona os dados fornecidos à planilha, se houver.

12. **Feedback na Console:**
    - Fornecimento de mensagens informativas na console durante o processo.

13. **Manipulação de Exceções:**
    - Captura exceções durante a criação do arquivo ou manipulação dos dados e imprime mensagens de erro na console.

14. **Método `checkExcelFile`:**
    - Assinatura: `private static boolean checkExcelFile(String directory, String fileName)`.
    - Verifica se o arquivo Excel existe no diretório especificado.

15. **Método `main`:**
    - Exemplo de uso da função `createExcelFile` com dados de exemplo.

16. **Saída na Console:**
    - A saída na console fornece informações sobre cada etapa do processo, desde a verificação da existência do arquivo até a criação bem-sucedida.
