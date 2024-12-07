
# Tabela Fipe API

Este é um projeto Java desenvolvido com **Spring Boot** que consome a API pública da Tabela Fipe para buscar informações sobre veículos como carros, motos e caminhões. Ele permite consultar marcas, modelos, anos e valores de veículos de forma interativa.

## 🚀 Funcionalidades

- **Consulta interativa**: Permite selecionar entre carros, motos ou caminhões.
- **Exibição de marcas**: Exibe as marcas disponíveis para a categoria escolhida.
- **Exibição de modelos**: Lista os modelos disponíveis para a marca selecionada.
- **Filtragem de modelos**: Filtra modelos com base em um termo fornecido.
- **Consulta por ano**: Exibe os valores dos veículos filtrados de acordo com o ano.

## 🛠️ Tecnologias Utilizadas

- **Java 23**
- **Spring Boot 3.4.0**
- **HTTPClient**: Para fazer requisições HTTP.
- **Jackson**: Para manipulação de dados JSON.

## ⚙️ **Como Executar**

1. Clone este repositório:

   ```bash
   git clone https://github.com/andradejohnny/Consulta_Tabela_Fipe.git
   ```


2. **Compile e execute o programa**:

   ```bash
   javac Main.java
   java Main
   ```

4. **Siga as instruções no terminal**:
   - Escolha a categoria do veículo (Carro, Moto ou Caminhão).
   - Navegue pelas marcas, modelos e anos.

   
## 📂 Estrutura do Projeto

O projeto está organizado em pacotes para uma maior legibilidade e modularidade.

### 📂 Pacotes

1. **`model`**: 
   - Contém as classes `Dados`, `Modelos` e `Veiculo`, que representam as entidades retornadas pela API.


2. **`service`**: 
   - `ConsumoApi`: Faz as requisições à API.
   - `ConverteDados` e `IConverteDados`: Convertem JSON para objetos Java e listas.


3. **`principal`**: 
   - `Principal`: Contém a lógica principal do programa.


4. **`application`**:
   - `TabelaFipeApplication`: Classe principal que inicializa o Spring Boot e executa a aplicação.

## Requisitos para Execução

- Java 17 ou superior instalado.
- Maven instalado para gerenciar as dependências.


## Exemplo de Execução

```plaintext
Insira uma das opções para consultar:

1 - Moto
2 - Carro
3 - Caminhão
> moto

[Exibição das marcas de motos]

Informe o código da marca:
> 1

[Exibição dos modelos da marca escolhida]

Informe o nome do veículo:
> cg

[Filtragem dos modelos contendo "cg"]

Digite o código do modelo do seu veículo:
> 125

[Exibição dos valores por ano]
```

## 📋 **Dependências**

1. Ter o [Java JDK](https://www.oracle.com/java/technologies/javase-downloads.html) instalado.
2. Configurar uma IDE como [IntelliJ IDEA](https://www.jetbrains.com/idea/) ou [Eclipse](https://www.eclipse.org/).
3. Adicionar a biblioteca Jackson Databind ao projeto.
   - **Maven**: Adicione a dependência abaixo ao seu `pom.xml`:
     ```xml
      <dependency>
         <groupId>com.fasterxml.jackson.core</groupId>
         <artifactId>jackson-databind</artifactId>
         <version>2.17.3</version>
      </dependency>

     ```

## Contribuições

Contribuições são bem-vindas! Caso queira melhorar o projeto, basta criar um **fork** deste repositório, realizar as mudanças e enviar um **pull request**.

**Desenvolvido com 💻 e ☕ por [ Johnny Andrade - https://github.com/andradejohnny ].**