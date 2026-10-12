import java.util.Scanner;
public class Main {
    public static void main(String[] args) {
        Scanner s = new Scanner(System.in);
        System.out.print("Piensa en un número límite máximo: ");

        int limite = s.nextInt();
        //limite: Guarda el número máximo//

        System.out.println("Generando 5 números especiales bajo el límite...");

        for (int i = 0; i < 5; i++) {
            //for: Repite el proceso cinco veces//

            int resultado = (int) (Math.random() * limite) + 1;
            //Math.random(): Genera un número aleatorio//
            //(int): Convierte el resultado a entero//

            System.out.println("Número [" + (i + 1) + "]: " + resultado);
            //+ 1: Hace que el resultado comience desde 1//
            //println: Muestra cada número generado//
        }

        s.close();
    }
}
//El programa solicita un límite máximo y genera cinco números aleatorios
// menores o iguales a ese límite.