# Laboratórios de POO · Java

![Java](https://img.shields.io/badge/Java-ED8B00?logo=openjdk&logoColor=white)
![License](https://img.shields.io/badge/license-MIT-blue)

Laboratórios e estudos de caso da disciplina de **Programação Orientada a Objetos** (Sistemas de Informação, IFMA). Cada pasta é um exercício independente, com as classes do problema e uma classe de teste com `main` para executar.

---

## Conteúdo

| Pasta | Tema | O que foi praticado |
|---|---|---|
| [Lab01](Lab01) | Classes e objetos | Primeiras classes com atributos e métodos: `Automovel`, `Pessoa` e uma simulação de `PopulacaoDeBaratas` |
| [Lab02](Lab02) | Encapsulamento | Conta bancária com `Cliente` e `Cartao`, atributos privados e métodos de acesso |
| [Lab03](Lab03) | Associação entre objetos | `Sensor` associado e desassociado de um `Controlador` |
| [Lab04](Lab04) | Composição | Conta bancária com histórico de lançamentos (`HistoricoDeLancamentos` e `Lancamento`) |
| [Lab05](Lab05) | Herança | `Ponto3D` e `Pixel` herdando de `Ponto2D` |
| [Lab06](Lab06) | Herança e polimorfismo | Funcionários (`Gerente`, `Desenvolvedor`, `Secretaria`), membros estáticos e um simulador de logística com veículos de carga |
| [Lab07](Lab07) | Interfaces | `Tributavel` para cálculo de imposto de renda e `ISimpleStack` com uma pilha de tamanho fixo e outra dinâmica |
| [Lab08](Lab08) | Classes abstratas e múltiplas interfaces | Plataforma EduTech: `ConteudoDigital` abstrata e conteúdos que implementam `Reproduzivel`, `Avaliavel`, `Imprimivel` e `ChatAoVivo` |
| [Lab09](Lab09) | Coleções | `List`, `Map`, `Iterator`, `Comparable` e `Comparator` num catálogo de produtos e num gerenciador de notas |
| [Lab10](Lab10) | Coesão e responsabilidades | Dívidas, pagamentos e um relatório com formatação de moeda por `Locale` |
| [EstudoDeCaso01](EstudoDeCaso01) | Caixa eletrônico | Contas, clientes, histórico de lançamentos e um terminal de caixa eletrônico |
| [EstudoDeCaso02](EstudoDeCaso02) | Leilão | Gestão de lotes, lances e pessoas num sistema de leilão |

---

## Como executar

**Pré-requisito:** JDK instalado.

Os pacotes começam no nome da pasta de cada lab (`package Lab05;`, `package Lab07.Atividade01;` etc.). Por isso, compile e execute **a partir da raiz do repositório**. Exemplo com o Lab05:

```bash
javac -d out Lab05/*.java
java -cp out Lab05.Teste
```

Nos labs com subpastas de atividades, aponte para a atividade:

```bash
javac -d out Lab07/Atividade01/*.java
java -cp out Lab07.Atividade01.Teste
```

O **Lab06** e o **Lab09** são exceções: os pacotes começam na atividade (`package Atividade01;`), então compile de dentro da pasta do lab:

```bash
cd Lab06
javac -d ../out Atividade01/*.java
java -cp ../out Atividade01.Teste
```

Também dá para abrir a pasta numa IDE (VS Code, IntelliJ ou Eclipse) e rodar a classe de teste de cada lab.

---

Distribuído sob a licença [MIT](LICENSE).
