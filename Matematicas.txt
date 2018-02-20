import java.util.Scanner;

public class Matematicas {
    public static void main(String[] args) {
        Scanner S = new Scanner (System.in);
        double pi = 3.14;
        double area, per;
        System.out.println ("¿Que figura desea escoger?");
        System.out.println ("1. Circulo");
        System.out.println ("2. Cuadrado");
        System.out.println ("3. Triangulo");
        System.out.println ("-------------------------------");
        int opc = S.nextInt ();        
        switch (opc){
            case 1:{
                System.out.println ("Ingrese el tamaño del radio: ");
                double rad = S.nextDouble ();
                area = pi*(rad*rad); 
                per = 2*pi*rad;
                System.out.println ("El area del circulo es: "+area);
                System.out.println ("El perimetro del circulo es: "+per);
                break;
            }
            case 2:{
                System.out.println ("Ingrese el tamaño del lado: ");
                double lad = S.nextDouble ();
                area =  lad*lad;            
                per = lad+lad+lad+lad;
                System.out.println ("El area del cuadrado es: "+area);
                System.out.println ("El perimetro del cuadrado es: "+per);
                break;
            }
            case 3:{
                System.out.println ("Ingrese el tamaño del lado: ");
                double lad = S.nextDouble ();
                System.out.println ("Ingrese el tamaño de la altura: ");
                double alt = S.nextDouble ();
                System.out.println ("Ingrese el tamaño de la base: ");
                double bas = S.nextDouble ();
                area = (bas*alt)/2;       
                per = lad+lad+lad;
                System.out.println ("El area del cuadrado es: "+area);
                System.out.println ("El perimetro del cuadrado es: "+per);
                break;
            }    
        }
    }
    
}