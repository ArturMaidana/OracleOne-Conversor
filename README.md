# 💱 Conversor de Moedas com Java e Gson

Projeto desenvolvido como parte do desafio da formação **Oracle One - Alura**, com o objetivo de construir um **Conversor de Moedas** utilizando **Java**, **API de câmbio** e a biblioteca **Gson** no **IntelliJ IDEA**.

---

## 🚀 Tecnologias Utilizadas

- Java 21
- API de taxas de câmbio (ex: [ExchangeRate API](https://www.exchangerate-api.com/))
- Gson (Google)
- IntelliJ IDEA

---

## 📋 Funcionalidades

- Consulta de taxas de câmbio em tempo real
- Conversão entre moedas diversas (ex: USD, EUR, BRL etc.)
- Interface via terminal com menu interativo
- Utilização de HTTP Client, HTTP Request e HTTP Response
- Análise e mapeamento de JSON com Gson

---

## 🧩 Etapas do Desenvolvimento

### 1. 📡 Integração com a API

- Estudo da documentação da API
- Geração da chave de acesso
- Testes de requisição via Postman

### 2. 📦 Importação da Biblioteca Gson

- Download do arquivo `gson-2.10.1.jar`
- Adição manual ao projeto:
  1. Vá em `File > Project Structure > Modules > Dependencies`
  2. Clique em `+` > `JARs or directories`
  3. Selecione o `.jar` do Gson
  4. Marque a opção **"Jar Directory"**

### 3. 🌐 Requisições HTTP com Java

- Uso do `HttpClient` para enviar requisições
- Configuração do `HttpRequest` com URL, headers e método `GET`
- Tratamento de `HttpResponse` com captura do corpo da resposta

### 4. 🧪 Manipulação de JSON com Gson

- Mapeamento de resposta JSON para objetos Java (records)
- Uso de `@SerializedName` para acessar os campos corretamente
- Filtros para extrair apenas as moedas de interesse

### 5. 💰 Conversão de Moedas

- Lógica para cálculo entre moedas com base na taxa recebida
- Métodos reutilizáveis e organizados para modularização do código

### 6. 🖥️ Interface via Console

- Menu com opções numéricas
- Entrada de dados com `Scanner`
- Laço de repetição até o usuário optar por sair
- Exibição do resultado final da conversão

---

## 📸 Demonstração (opcional)

```bash
Selecione uma moeda base:
1 - USD
2 - EUR
3 - BRL

Digite o valor que deseja converter:
> 100

Resultado: 100 USD = 523.45 BRL
