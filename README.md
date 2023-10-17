### ExcelFileHandler Class

A classe `ExcelFileHandler` fornece métodos para manipulação de arquivos Excel (.xlsx), incluindo criação de arquivos, verificação de existência e transporte de dados para planilhas.

#### Uso Básico

Aqui está um exemplo de como utilizar a classe `ExcelFileHandler`:

```java
public class ExemploDeUso {

    public static void main(String[] args) {
        // Defina o diretório, nome do arquivo e nome da planilha Excel
        String directory = "src/bd/";
        String fileName = "Key";
        String sheetName = "users";

        // Defina os dados da célula (se necessário)
        String[][] cellData = {
            {"Name", "Password", "Date"},
            {"Enrique", "1234A", "12/10/23"}
        };

        // Chame o método para criar o arquivo Excel
        ExcelFileHandler.createExcelFile(directory, fileName, sheetName, cellData);
    }
}
```

#### Descrição dos Métodos

- **`createExcelFile`**
  - Cria um arquivo Excel (.xlsx) no diretório especificado e adiciona dados à planilha, se fornecidos.
  - Parâmetros:
    - `directory`: O diretório onde o arquivo será criado.
    - `fileName`: O nome do arquivo Excel.
    - `sheetName`: O nome da planilha Excel.
    - `cellData`: Dados a serem inseridos nas células no formato `{{"Dado1", "Dado2", ...}, {"Valor1", "Valor2", ...}}`.

- **`checkExcelFile`**
  - Verifica se um arquivo Excel (.xlsx) existe no diretório especificado.
  - Parâmetros:
    - `directory`: O diretório onde o arquivo é verificado.
    - `fileName`: O nome do arquivo Excel.

#### Observações
- Certifique-se de ter a biblioteca Apache POI no seu caminho de classe para utilizar esta classe corretamente. Você pode baixá-la em [Apache POI](https://poi.apache.org/download.html).

- Adapte os valores dos parâmetros conforme necessário para a integração com seu projeto.
