# Testes Automatizados para o Projeto

Este repositório contém os testes automatizados para o projeto. Os testes são divididos em três partes principais:

1. **Testes Funcionais de API** usando **Postman**.
2. **Testes Funcionais de Interface Web** usando **Selenium**.
3. **Testes de Performance** usando **JMeter**.

## 1. Testes Funcionais de API com Postman

### Como usar os arquivos Postman:
1. **Importar a Coleção**:
   - Abra o **Postman**.
   - Clique em **Import** no canto superior esquerdo.
   - Selecione o arquivo `api_tests.json` e importe para o Postman.

2. **Ambiente**:
   - Se você tiver variáveis de ambiente, crie um novo **Ambiente** no Postman e adicione as variáveis conforme necessário, como `localhost` ou variáveis de autenticação.
   
3. **Executar os Testes**:
   - Selecione a coleção importada.
   - Clique em **Run** para iniciar os testes de API.
   - Os testes incluirão endpoints como `/consulta/cadastro`, `/sinistro/cadastro`, entre outros.
   
4. **Verificar os Resultados**:
   - O Postman exibirá os resultados de cada request.
   - Verifique os status das requisições e se os testes passaram ou falharam.

---

## 2. Testes Funcionais de Interface Web com Selenium

### Como usar os testes Selenium com a extensão do navegador:

1. **Instalar a Extensão Selenium IDE**:
   - Para usar os testes de Selenium, você precisa instalar a extensão **Selenium IDE** no seu navegador:
     - **Google Chrome**: [Instalar Selenium IDE no Chrome](https://chrome.google.com/webstore/detail/selenium-ide)
     - **Mozilla Firefox**: [Instalar Selenium IDE no Firefox](https://addons.mozilla.org/en-US/firefox/addon/selenium-ide/)

2. **Importar o Arquivo `.side`**:
   - Abra o **Selenium IDE** no seu navegador.
   - No Selenium IDE, clique em **Open Project** e selecione o arquivo `.side` (por exemplo, `cadastro_consulta.side` ou `cadastro_sinistro.side`) que está na pasta `selenium_tests/`.

3. **Executar os Testes**:
   - Após importar o arquivo `.side`, você verá os passos de automação gravados.
   - Clique em **Run** no Selenium IDE para executar os testes. O Selenium IDE irá interagir com o seu aplicativo web, realizando as ações de cadastro de consulta ou sinistro conforme gravado.

4. **Verificar os Resultados**:
   - O Selenium IDE exibirá os resultados de execução diretamente na interface, mostrando se os testes passaram ou falharam.
   - Você também pode visualizar logs detalhados e mensagens de erro para identificar problemas nos testes.

---

## 3. Testes de Performance com JMeter

### Como usar os testes JMeter:
1. **Instalar o JMeter**:
   - Baixe e instale o **Apache JMeter** no [site oficial](https://jmeter.apache.org/).

2. **Configuração do Teste**:
   - Navegue até a pasta `jmeter_tests/`.
   - Abra o arquivo `.jmx` (por exemplo, `cadastro_consulta.jmx`) no **JMeter**.
   - O teste irá simular usuários realizando o cadastro de consultas ou sinistros, com o foco em medir o tempo de resposta e a taxa de erro.

3. **Configuração de Usuários Virtuais**:
   - O teste foi configurado para simular um volume de **20 a 50 usuários virtuais**.
   - O tempo de execução foi definido para **1 minuto**.
   - O JMeter irá coletar métricas como **tempo de resposta**, **throughput** e **erros**.

4. **Executar o Teste**:
   - Após abrir o arquivo `.jmx` no JMeter, clique em **Run** para executar os testes.
   - Os resultados serão exibidos no painel do JMeter, e você pode visualizar gráficos, métricas de performance e detalhes dos erros.

5. **Gerar Relatórios**:
   - Após a execução, você pode gerar relatórios de desempenho, visualizando as métricas de cada cenário de teste.
   - O JMeter também permite comparar múltiplos cenários, fornecendo uma visão clara da performance da aplicação sob diferentes cargas.

---

## Alunos

- Luana Sousa Matos 552621
- Nicolas Martins 553478

---

## Vídeo

https://drive.google.com/drive/folders/1kVwBLs3gNexJLw6VdyFhlK8l_sIDm776?usp=sharing
