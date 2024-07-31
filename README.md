# Loja Online

Este projeto é um sistema simples de gerenciamento de loja online implementado em Java usando os princípios de Programação Orientada a Objetos (POO). Ele permite criar produtos, clientes, itens de pedidos e pedidos, encapsulando dados e comportamentos específicos ao seu domínio.

## Estrutura do Projeto

O projeto é composto pelas seguintes classes:

- **Produto**: Representa um produto com nome, preço e quantidade em estoque.
- **Cliente**: Representa um cliente com nome, e-mail e telefone.
- **ItemPedido**: Representa um item de um pedido, associando um produto à quantidade comprada.
- **Pedido**: Representa um pedido feito por um cliente, contendo uma lista de itens e a data do pedido.

## Classes

### Produto

```java
public class Produto {
    private String nome;
    private double preco;
    private int estoque;

    public Produto(String nome, double preco, int estoque) {
        this.nome = nome;
        this.preco = preco;
        this.estoque = estoque;
    }

    public String getNome() {
        return nome;
    }

    public double getPreco() {
        return preco;
    }

    public int getEstoque() {
        return estoque;
    }

    public void setEstoque(int estoque) {
        this.estoque = estoque;
    }

    @Override
    public String toString() {
        return "Produto{" +
                "nome='" + nome + '\'' +
                ", preco=" + preco +
                ", estoque=" + estoque +
                '}';
    }
}
