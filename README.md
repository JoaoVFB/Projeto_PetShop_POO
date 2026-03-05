# Sistema de Gerenciamento para Pet Shop

## Descrição do Projeto

Este projeto consiste em um sistema de gerenciamento para Pet Shop desenvolvido em **Java** utilizando a biblioteca **Java Swing** para a interface gráfica. O objetivo principal foi aplicar os conceitos de **Programação Orientada a Objetos (POO)**, o padrão de projeto **Singleton** e técnicas de **Tratamento de Erros** para criar uma aplicação robusta e de fácil utilização.

O sistema permite o cadastro e gerenciamento de serviços como banho, tosa e tosa higiênica, além de gerenciar informações de clientes e animais. A arquitetura do projeto foi pensada para demonstrar a aplicação de princípios de POO, como herança e polimorfismo, e o uso do padrão Singleton para garantir uma única instância de classes de gerenciamento de dados.

## Funcionalidades

As principais funcionalidades do sistema incluem:

*   **Cadastro de Clientes e Animais:** Registro de informações detalhadas sobre os tutores e seus pets.
*   **Agendamento de Serviços:** Marcação de banhos, tosas e tosas higiênicas com controle de datas e horários.
*   **Gerenciamento de Serviços:** Inclusão, consulta, atualização e exclusão de serviços oferecidos.
*   **Tratamento de Exceções:** Implementação de classes de exceção personalizadas para lidar com entradas inválidas (e.g., idade negativa, nome numérico).

## Tecnologias Utilizadas

*   **Java:** Linguagem de programação principal.
*   **Java Swing:** Para o desenvolvimento da interface gráfica de usuário (GUI).

## Conceitos de POO Aplicados

*   **Herança:** Classes como `Banho`, `Tosa` e `TosaHigienica` herdam de uma classe base `Servico`, promovendo a reutilização de código e a organização hierárquica.
*   **Polimorfismo:** Métodos sobrescritos nas classes filhas para implementar lógicas específicas de cada tipo de serviço.
*   **Encapsulamento:** Uso de modificadores de acesso (`private`, `public`) para proteger os dados e controlar o acesso aos atributos das classes.
*   **Abstração:** A classe `Servico` é abstrata, definindo um contrato para os serviços sem especificar a implementação completa.

## Padrão de Projeto Singleton

O padrão **Singleton** foi aplicado nas classes de banco de dados (`BDbanho`, `BDtosa`, `BDtosaHig`) para garantir que exista apenas uma instância dessas classes em toda a aplicação. Isso é crucial para gerenciar de forma centralizada as coleções de dados dos serviços, evitando inconsistências e otimizando o uso de recursos.

## Tratamento de Erros

O projeto incorpora um robusto tratamento de erros com a criação de exceções personalizadas, como:

*   `IdadeNegException`
*   `NomeNegException`
*   `NumNegException`
*   `RacaNumException`

Essas exceções são lançadas e tratadas para garantir a integridade dos dados inseridos pelo usuário e proporcionar uma experiência mais amigável, informando sobre entradas inválidas.

## Estrutura do Projeto

```
ProjetoPetShop/
├── src/
│   └── main/
│       └── java/
│           ├── Agendamento.java
│           ├── Animal.java
│           ├── Banho.java
│           ├── BDbanho.java
│           ├── BDtosa.java
│           ├── BDtosaHig.java
│           ├── Cliente.java
│           ├── Duracao.java
│           ├── FormAtuBa.java
│           ├── FormAtuTo.java
│           ├── FormAtuToH.java
│           ├── FormBanho.java
│           ├── FormConsBa.java
│           ├── FormConsTo.java
│           ├── FormConsToH.java
│           ├── FormPrincipal.java
│           ├── FormTosa.java
│           ├── FormTosaHig.java
│           ├── IdadeNegException.java
│           ├── NomeNegException.java
│           ├── NumNegException.java
│           ├── RacaNumException.java
│           ├── Servico.java
│           ├── Tosa.java
│           └── TosaHigienica.java
└── pom.xml 
```

## Como Rodar o Projeto

1.  **Clone o repositório:**
    ```bash
    git clone <URL_DO_SEU_REPOSITORIO>
    ```
2.  **Abra o projeto em uma IDE Java:** Importe o projeto para sua IDE preferida (e.g., IntelliJ IDEA, Eclipse, NetBeans).
3.  **Compile e Execute:** A partir da IDE, compile e execute a classe `FormPrincipal.java` para iniciar a aplicação.

## Screenshots
Demonstração do agendamento de um serviço do tipo banho.
### Tela de menu principal
<img width="632" height="377" alt="Tela_Principal" src="https://github.com/user-attachments/assets/f6b829f9-f9ad-4e09-9815-649cc09bcd1f" />


### Tela de cadastro
<img width="691" height="797" alt="Tela_cadastro" src="https://github.com/user-attachments/assets/cef7de6c-2ea5-4659-a3dd-db6c6aa2b6e1" />

### Feedback ao realizar um agendamento com sucesso
<img width="318" height="166" alt="AgendamentoRealizado" src="https://github.com/user-attachments/assets/888c8379-c7f6-4387-8f7b-e27d65fe7e3e" />

### Tabela com os agendamentos
<img width="1312" height="523" alt="TabelaDeAgendamentos" src="https://github.com/user-attachments/assets/7939532a-2206-4f30-90d5-468845f7d677" />

## Aprendizado
Ao construir este projeto do início, fortaleci minhas habilidades analíticas e de resolução de problemas. A aplicação prática foi crucial para solidificar o domínio em Java e nos pilares da Programação Orientada a Objetos.
