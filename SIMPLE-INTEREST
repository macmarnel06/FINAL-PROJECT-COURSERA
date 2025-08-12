/* Programa Simple Socket Factory Client */

// Observe que se importa javax.net.* para tomar la clase SocketFactory.
import javax.net.*; 
import java.net.*;
import java.io.*;

public class factorySocketClient {
  public static void main (String args[]) throws IOException {

    int serverPort = 3000;

    if (args.length < 1) {
      System.out.println("java factorySocketClient serverHost serverPort");
      System.out.println("serverPort toma por defecto 3000 si no se especifica.");
      return;
    }
    if (args.length == 2)
      serverPort = new Integer(args[1]).intValue();

    System.out.println("Conectando a host " + args[0] + " en el puerto " +
                       serverPort);

    // Cambiar el programa simpleSocketClient original para crear una
    // fábrica de sockets y luego utilizarla para crear sockets.

    SocketFactory socketFactory = SocketFactory.getDefault();

    // Ahora, la fábrica crea el socket.  Es el último cambio
    // que se realiza en el programa simpleSocketClient original.

    Socket  s = socketFactory.createSocket(args[0], serverPort);
    .
    .
    .
    
    // El resto del programa sigue a partir de aquí.
