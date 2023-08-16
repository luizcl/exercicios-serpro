# Exercícios de preparação para o SERPRO

## 1) [Simulado do estratégia](https://github.com/raphaelLacerda/java-treino-programacao)
 - Descrição:
  - Realizar um CRUD
  - Corrigir bug
  - Refatorar código
  - Testar código (Fake, Stub e Mock)

## 2) [Simulado 1 do Youtube](https://www.youtube.com/watch?v=kvmHQKJxmns)
 - Utilizando o node, corrigir e implementar funcionalidades novas

## 3) [Simulado 2 do Youtube](https://youtu.be/YqNVgqiA3DQ)
 > O desafio consiste em criar um módulo básico de Kanban. A ideia se originou de uma prova discursiva aplicada para Auditor de Controle Externo - TI.
Embora a banca do concurso do SERPRO seja a CEBRASPE, eu peguei a questão discursiva da FGV, já que vi um cenário que faz mais sentido para a prova prática do SERPRO.

## 4) Aplicação do Padrão Singleton:

 - Dado o seguinte trecho de código para uma classe de configuração:
```Java
public class Configuration {
    public String apiUrl;
    public int timeout;

    public Configuration() {
        apiUrl = "https://api.example.com";
        timeout = 5000;
    }
}
```

## 5) Implementação de Ordenação Binária:

```Java
int[] numbers = {15, 3, 9, 7, 23, 4};

```
 - Escreva um código  que implemente a ordenação binária (como o heapsort) para ordenar esse array em ordem crescente.

## 6) Aplicação do Padrão Factory Method:

 - Considere o seguinte código que representa uma classe abstrata Product e duas classes concretas ProductA e ProductB:

```Java
abstract class Product {
    public abstract void create();
}

class ProductA extends Product {
    public void create() {
        System.out.println("Creating Product A");
    }
}

class ProductB extends Product {
    public void create() {
        System.out.println("Creating Product B");
    }
}
```

 - Adapte o código acima para utilizar o padrão Factory Method, de forma a permitir a criação de objetos ProductA ou ProductB sem expor as classes concretas ao código cliente.


## 7) Refatoração Usando Padrão Strategy:

 - Dado o seguinte trecho de código:

```Java
class TaxCalculator {
    public double calculateTax(String type, double amount) {
        if (type.equals("VAT")) {
            return amount * 0.2;
        } else if (type.equals("GST")) {
            return amount * 0.18;
        }
        return 0;
    }
}
```

 - Refatore o código acima utilizando o padrão Strategy, de forma a tornar a classe TaxCalculator mais flexível e extensível para diferentes tipos de impostos.

## 8) Prova antiga IFMG:
 - [Ver o PDF](https://raw.githubusercontent.com/luizcl/exercicios-serpro/main/files/Prova%20Pr%C3%A1tica%20-%20%C3%81rea%20Desenvolvimento.pdf)

## 9) Questão Telegram - Dia 1:
 - Contexto:
   - Uma instituição de ensino deseja desenvolver um sistema simples de gerenciamento de alunos. Este sistema deve ser capaz de armazenar informações básicas dos alunos, como nome, matrícula e notas das disciplinas cursadas.

 - Requisitos:
    - O sistema deve permitir a inserção de um novo aluno, com nome e número de matrícula.
    - Deve ser possível inserir notas para cada aluno em disciplinas específicas.
    - O sistema deve listar todos os alunos e suas respectivas notas.
    - Deve ser possível calcular a média das notas de um aluno.
    - O sistema deve identificar e listar alunos com média abaixo de 7.0, considerando-os como "em recuperação".

  - Resolver:
    - 1: Desenvolver um programa que permita a inserção de um novo aluno com as informações de nome e matrícula. (Avaliação da funcionalidade básica do sistema)
    - 2: Expanda o programa anterior para que possa inserir notas para cada aluno em disciplinas específicas. (Manipulação de estruturas de dados)
    - 3: Desenvolva uma funcionalidade que liste todos os alunos e suas respectivas notas. (Manipulação e exibição de dados)
    - 4: Implemente uma função que calcule a média das notas de um aluno específico. (Cálculo e manipulação de dados)
    - 5: No código a seguir, identifique e corrija os erros que impedem o correto funcionamento do sistema. (Análise e correção de código-fonte)
    - 6: Refatore o código acima para que esteja de acordo com as boas práticas de desenvolvimento, mantendo a sua funcionalidade. (Refatoração e Clean Code)
    - 7: Desenvolva um teste unitário para validar a funcionalidade de cálculo da média das notas de um aluno. (Elaboração de testes)
 
```Java
public class Aluno {
    private String nome;
    privte int matricula;
    private double nota1, nota2, nota3;
    
    public String getNome() {
        return nome
    }
    
    public void setNome(String nome) {
        this.nome = nome;
    }
    
    public int getMatricula() {
        return matricula;
    }
    
    public void setMatricula(int matricula) {
        this.matricula == matricula;
    }
    
    public double calculaMedia() {
        return (nota1 + nota2 + nota3) / 2;
    }
}
```
 - Instruções:
   - Utilize a linguagem Java para o desenvolvimento da solução.
   - Atenção à sintaxe e boas práticas de programação.
   - Avalie o resultado (saída do software) e garanta a correta execução do software a partir dos requisitos descritos.
  
## 10) Questões Telegram - Dia 2:

 - Contexto:
   - Uma empresa financeira deseja desenvolver um sistema de gerenciamento de transações. Esse sistema será responsável por registrar, listar e analisar transações financeiras realizadas por seus clientes em diferentes modalidades e moedas.


 - Requisitos:
   - O sistema deve permitir a inserção de uma nova transação financeira com os seguintes dados: cliente, valor, moeda (USD, EUR, BRL, etc.) e tipo de transação (Depósito, Retirada, Transferência).
   - Deve ser possível filtrar e listar transações por cliente e/ou tipo de transação.
   - O sistema deve calcular a taxa de câmbio para transações em moedas estrangeiras.
   - Deve ser possível calcular o saldo total de um cliente em sua moeda local.
   - Implementar um mecanismo de detecção de transações suspeitas. Uma transação é considerada suspeita se um cliente realiza três ou mais retiradas num período de 24 horas.

 - Resolver:
   - Questão 1: Desenvolva uma classe Transacao que represente uma transação financeira, considerando os atributos e métodos necessários para atender aos requisitos acima.
   - Questão 2: Desenvolva uma funcionalidade que permita filtrar e listar transações por cliente e/ou tipo de transação, usando estruturas de dados eficientes para filtragem e ordenação.
   - Questão 3: Implemente uma classe ConversorMoeda que use uma API externa (ou uma simulação de uma) para pegar as taxas de câmbio atualizadas e realize a conversão entre diferentes moedas.
   - Questão 4: No sistema, crie uma funcionalidade que, ao consultar o saldo total de um cliente, faça a conversão de todas as suas transações para sua moeda local, considerando as taxas de câmbio do dia.
   - Questão 5: Implemente a detecção de transações suspeitas. Crie testes unitários para validar essa funcionalidade.
   - Questão 6: O código a seguir é parte do sistema de transações. Identifique possíveis falhas de performance, vulnerabilidades ou erros e corrija-os, detalhando cada problema encontrado e sua solução:
   - Questão 7: Suponha que o sistema tenha que lidar com milhões de transações diariamente. Propor e justificar otimizações no design do sistema e/ou no uso de tecnologias específicas para garantir eficiência e escalabilidade.

```Java
public class Transacao {
    public String cliente;
    public double valor;
    public String moeda;
    public String tipo;
    
    public List<Transacao> todasTransacoes = new ArrayList<>();

    public void adicionarTransacao(Transacao t) {
        todasTransacoes.add(t);
    }
    
    public double getSaldo(String cliente) {
        double saldo = 0.0;
        for (Transacao t : todasTransacoes) {
            if (t.cliente.equals(cliente)) {
                saldo += t.valor;
            }
        }
        return saldo;
    }
}
```

 - Instruções:
   - Utilize a linguagem Java para o desenvolvimento da solução.
   - Atenção às práticas de programação segura, principalmente ao lidar com informações financeiras.
   - Avalie a saída do software e garanta a correta execução do software a partir dos requisitos descritos.


## 10) Questões Telegram - Dia 3:

 - Dica - Resolvam primeiro o dia 3, o Dia 2 precisa de SpringBoot e JPA pra ser resolvido com eficiência.
 - Contexto:
   - O Serpro está com problemas de desempenho e precisa aumentar a eficiência de suas buscas e você ficou encarregado de testar a implementação de algoritmos de ordenação e estruturas de árvores binárias.

  - Resolver:
    - Questão 1: Ordenação
      - Dado o seguinte array de produtos:
      - ```Java
        [“Celular”, “Notebook”, “Televisão”, “Tablet”, “Câmera”, “Smartwatch”]
        ```
        - a) Implemente um algoritmo de ordenação por seleção (Selection Sort) para ordenar os produtos em ordem alfabética.
        - b) Apresente a quantidade de comparações e trocas realizadas durante o processo de ordenação.
    - Questão 2: Árvore Binária de Busca
      - Suponha que cada produto tenha um código numérico associado:
        - > Celular: 5
          > 
          > Notebook: 3
          > 
          > Televisão: 8
          > 
          > Tablet: 1
          > 
          > Câmera: 4
          > 
          > Smartwatch: 7
          - a) Utilizando os códigos numéricos acima, insira os produtos em uma árvore binária de busca.
          - b) Descreva a sequência de inserção dos produtos para que a árvore binária de busca esteja balanceada.
          - c) Escreva um algoritmo para encontrar um produto pelo seu código na árvore.

    - Questão 3: Balanceamento de Árvore
      - Tendo a árvore binária de busca anteriormente criada:
        - a) Verifique se a árvore está balanceada.
        - b) Se não estiver balanceada, aplique o algoritmo de rotação à direita para balancear a árvore.
        - c) Apresente a nova estrutura da árvore após o balanceamento.

    - Questão 4: Ordenação com Árvore
      - Dado o seguinte array de vendas do mês:
        - > [1500, 900, 2100, 300, 2800, 750, 1800]
          - a) Insira os valores na árvore binária de busca.
          - b) Implemente o algoritmo de "pre-ordem" para extrair os valores da árvore em ordem crescente, efetivamente ordenando o array.
          - c) Liste os valores ordenados obtidos a partir do "pre-ordem".
