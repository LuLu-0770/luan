import java.util.Scanner;
public class Ac1 {

    public static void main(String[] args ){
        Scanner scanner = new Scanner(System.in);
        

        System.out.println("==========================");
        System.out.println("       Média Facens");
        System.out.println("==========================");
        System.out.println("Para começar, digite a sua nota da AC1: ");double AC1 = scanner.nextDouble();
        System.out.println("Agora, a sua nota na AC2: ");double AC2 = scanner.nextDouble();
        System.out.println("Sua nota na AG: ");double AG = scanner.nextDouble();
        System.out.println("Para finalizar, sua nota na AF: ");double AF = scanner.nextDouble();

        double media = (AC1* 0.15) + (AC2 *0.30) + (AG * 0.10) + (AF * 0.45); 
        double falta = -1*(media - 5);

        System.out.println("=============================");
        System.out.println("     Sua média foi de " + media);
        if (media >= 5) {
            System.out.println("=============================");
            System.out.println("     Você foi aprovado!");
            System.out.println("=============================");
        }else{  
            System.out.println("=============================");
            System.out.println("     Você foi reprovado. ");
            System.out.println("=============================");
            System.out.println("     Faltaram "+ falta + " pontos." );
            System.out.println("=============================");
      
        }
        
        System.out.println("Sua nota na AC1 foi de "+ AC1);
        System.out.println("Sua nota na AC2 foi de "+ AC2);
        System.out.println("Sua nota na AG foi de "+ AG);
        System.out.println("Sua nota na AF foi de "+ AF);
        scanner.close();
        




    }
    
}


