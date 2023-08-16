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
 - [Ver o PDF](http://localhost)
