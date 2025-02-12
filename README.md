package AULA1202;

import java.util.Scanner;

public class Viagem {
    public static void main(String[] args) {
        Scanner leia= new Scanner(System.in);

        //informações

        double kmviagem;
        double consumaVeiculo;
        double kmViagemIV;
        double precoCombustivel;
        double quantidadeLitros;
        double custo;
        String nomeCidade;


        System.out.println("preco combustivel:");
        precoCombustivel = leia.nextDouble();

        System.out.println("KM da viagem:");
        kmviagem = leia.nextDouble();
        kmViagemIV = kmviagem * 2;

        System.out.println("qual o consumo do veiculo:");
        consumaVeiculo = leia.nextDouble();

        System.out.println("nome da cidade:");
        nomeCidade = leia.next();

        quantidadeLitros = kmViagemIV / consumaVeiculo;

        custo = quantidadeLitros * precoCombustivel;

        System.out.println("o custo da viagem para " + nomeCidade + " vai ser de:R$:" + custo);


    }
}
