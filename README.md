import java.util.Scanner;

public class Main {
  public static void main(String[] args) {
   //Declarar variáveis
    int nota;
    Scanner entrada = new Scanner(System.in);
    do{
      // ler nota
      System.out.println("Informe a nota: ");
      nota = entrada.nextInt();
      if(nota < 0 || nota > 10 ){
        System.out.println("Nota inválida !");
      }
      
    }while(nota < 0 || nota > 10);

    System.out.println("Você informou a nota: "+ nota);
    // Destroy a instância do scanner
    entrada.close();
  }


}
