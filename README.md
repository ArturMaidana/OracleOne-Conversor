☕ Conversor de Moedas em Java
📖 Sobre o Projeto
Este é um conversor de moedas interativo desenvolvido em Java, que funciona diretamente no console. O projeto utiliza a API da ExchangeRate-API para obter as taxas de câmbio mais recentes em tempo real, garantindo conversões precisas.

A aplicação apresenta um menu simples e intuitivo, permitindo que o usuário escolha entre diferentes pares de moedas para conversão e insira o valor desejado.

✨ Funcionalidades
Menu Interativo: Interface de console amigável com um loop de repetição para múltiplas conversões.

Taxas de Câmbio em Tempo Real: Conecta-se a uma API externa para buscar dados atualizados.

Conversões Populares: Oferece opções de conversão pré-definidas entre moedas como Dólar (USD), Real Brasileiro (BRL), Euro (EUR) e Peso Argentino (ARS).

Código Limpo e Modular: O código é organizado em métodos que seguem as responsabilidades de cada etapa do processo:

Conexão com a API.

Análise da resposta (parsing de JSON).

Cálculo da conversão.

Interação com o usuário.

🛠️ Tecnologias Utilizadas
Java 17+: Linguagem principal do projeto.

Java HttpClient: Cliente HTTP nativo do Java (a partir do Java 11) para realizar as requisições à API.

Gson: Biblioteca do Google para converter objetos Java em sua representação JSON e vice-versa.

🚀 Como Executar o Projeto
Siga os passos abaixo para configurar e rodar a aplicação em seu ambiente local.

Pré-requisitos
JDK (Java Development Kit) 17 ou superior instalado.

IntelliJ IDEA ou outra IDE de sua preferência.

Uma chave de API da ExchangeRate-API. O plano gratuito é suficiente.

Configuração
Clone o Repositório

git clone https://github.com/seu-usuario/seu-repositorio.git

Importe a Biblioteca Gson no IntelliJ

Abra o projeto no IntelliJ.

Clique com o botão direito na pasta do projeto e selecione Open Module Settings.

Vá para a aba Libraries e clique no + para adicionar uma nova biblioteca From Maven....

Pesquise por com.google.code.gson:gson:2.10.1 e adicione ao projeto.

Adicione sua Chave de API

Abra o arquivo ConversorDeMoedas.java.

Encontre a seguinte linha:

String apiKey = "SUA_CHAVE_API";

Substitua "SUA_CHAVE_API" pela chave que você obteve no site da ExchangeRate-API.

Execução
Abra o arquivo ConversorDeMoedas.java.

Clique com o botão direito do mouse dentro do editor e selecione Run 'ConversorDeMoedas.main()'.

O programa será executado no console do IntelliJ.

💻 Exemplo de Uso
Ao iniciar, o programa exibirá o menu principal. Basta digitar o número da opção desejada, pressionar Enter, e em seguida fornecer o valor a ser convertido.

Buscando taxas de câmbio...
Taxas carregadas com sucesso!

***************************************************
Bem-vindo ao Conversor de Moedas!
1) Dólar (USD) =>> Real Brasileiro (BRL)
2) Real Brasileiro (BRL) =>> Dólar (USD)
3) Euro (EUR) =>> Real Brasileiro (BRL)
4) Real Brasileiro (BRL) =>> Euro (EUR)
5) Dólar (USD) =>> Peso Argentino (ARS)
6) Peso Argentino (ARS) =>> Dólar (USD)
7) Sair
Escolha uma opção válida:
***************************************************
1
Digite o valor que deseja converter: 150

150.00 USD equivalem a 765.00 BRL
