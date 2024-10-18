import java.util.Scanner;
public class gabrielTallerAutomotriz {
    public static void main(String[] args){
        Scanner gabriel = new Scanner(System.in);
    int opcion;
        do {
        System.out.println("Bienvenido al taller de Grifo Primax");
        System.out.println("Menu principal Taller:");
        System.out.println("Tenemos estas opciones:");
        System.out.println("Opcion 1: Cambio de aceite");
        System.out.println("Opcion 2: limpieza Veicular");
        System.out.println("Opcion 0: salir del taller");
        opcion = gabriel.nextInt();
        gabriel.nextLine();
        switch (opcion) {
            case 1:
                System.out.println("CAMBIO DE ACIETE");
                System.out.println("Precio: $ 149.90");
                double cambiodeaceite = 149.90;
                double igv = cambiodeaceite * 0.18;
                double subtotal;
                igv = (cambiodeaceite) * 0.18;
                subtotal = (cambiodeaceite) - igv;
                cambiodeaceite = subtotal + igv;

                System.out.println("cambio de aceite: ");
                System.out.println("Ud debe pagara $149.90");
                double pago = gabriel.nextInt();
                if (pago >= 149.90) {
                    if (pago > 149.90) {
                        double vuelto = pago - 149.90;
                        System.out.println("su vuelto es: " + vuelto);
                        System.out.println("*************");
                        System.out.println("Subtotal: " + subtotal);
                        System.out.println("igv(18%): " + igv);
                        System.out.println("TOTAL PAGAR: " + cambiodeaceite);
                        System.out.println("*************");
                    }
                    System.out.println("Gracias por pagar ahora empazamos a cambiar el aceite....");
                    gabriel.nextLine();
                    System.out.println("Espere por favor.....");
                    for (int i = 1; i <= 45; i++) {
                        System.out.println("minuto " + i);
                    }
                    System.out.println("Gracias por esperar hemos acabado");
                }
            case 2:
                System.out.println("LIMPIEZA VEHICULAR");
                System.out.println("Precio: 39.90");
                double limpiezavehicular = 39.90;
                double subtotaldelimpieza;
                igv = limpiezavehicular;
                igv = (limpiezavehicular * 0.18);
                subtotaldelimpieza = (limpiezavehicular) - igv;
                limpiezavehicular = subtotaldelimpieza + igv;

                System.out.println("limpieza vehicular ");
                System.out.println("Ud debe pagara $39.90");
                System.out.print("Ingrese el dinero:");
                double pagodelimpieza = gabriel.nextInt();
                if (pagodelimpieza >= 39.90) {

                    if (pagodelimpieza > 39.90) {
                        double vuelto = pagodelimpieza - 39.90;
                        System.out.println("su vuelto es: " + vuelto);
                        System.out.println("*************");
                        System.out.println("Subtotal: " + subtotaldelimpieza);
                        System.out.println("igv(18%): " + igv);
                        System.out.println("TOTAL PAGAR: " + limpiezavehicular);
                        System.out.println("*************");
                    }
                    System.out.println("Gracias por pagar ahora empazamos a cambiar el aceite....");
                    gabriel.nextLine();
                    System.out.println("Espere por favor.....");
                    for (int i = 1; i <= 25; i++) {
                        System.out.println("minuto " + i);
                    }
                    System.out.println("Gracias por esperar hemos acabado");
                } else {
                    System.out.println("Regresa con plata🤦‍♂️🤦‍♂️: ");
                    System.exit(0);
                }
            case 0:
                System.out.println("Estas regresando");
                break;
            default:
                System.out.println("Opcion fuera de rango");
                break;
        }
    }while (opcion !=0);
}
}
