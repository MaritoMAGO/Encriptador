# Encriptador
Encriptar y desencriptar en lenguaje Ascii

public class Encriptador {

    
    public static void main(String[] args) {
        
        String mensaje;
        String msjEncriptado;
        String msjDesencriptado;
        
        char array[];
        
        mensaje = JOptionPane.showInputDialog("Ingresar Texto");
        array = mensaje.toCharArray();
        
        for (int i = 0; i < array.length; i++)
        {
            array[i]=(char)(array[i]+(char)6);
        }
        
        msjEncriptado = String.valueOf(array);
        System.out.println("Texto a Encriptar");
        System.out.println(mensaje);
        System.out.println("Texto Encriptado");
        System.out.println(msjEncriptado);
        
         for (int i = 0; i < array.length; i++)
        {
            array[i]=(char)(array[i]-(char)6);
        }
        msjDesencriptado = String.valueOf(array);
        System.out.println("Texto Desencriptado");
        System.out.println(msjDesencriptado);
        
    }
