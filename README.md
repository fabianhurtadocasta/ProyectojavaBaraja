# ProyectojavaBaraja

// Código Java para barajar una baraja de cartas 
import java.util.Random; 
  
class JVC { 
      
    // Función que baraja e imprime el array
    public static void shuffle(int card[], int n) 
    { 
          
        Random rand = new Random(); 
          
        for (int i = 0; i < n; i++) 
        { 
            // Random for remaining positions. 
            int r = i + rand.nextInt(52 - i); 
              
             //swapping the elements 
             int temp = card; 
             card = card; 
             card = temp; 
               
        } 
    } 
       
    // Código del controlador 
    public static void main(String[] args)  
    { 
        // Array from 0 to 51 
        int a[] = {0, 1, 2, 3, 4, 5, 6, 7, 8, 
                   9, 10, 11, 12, 13, 14, 15, 
                   16, 17, 18, 19, 20, 21, 22, 
                   23, 24, 25, 26, 27, 28, 29, 
                   30, 31, 32, 33, 34, 35, 36, 
                   37, 38, 39, 40, 41, 42, 43, 
                   44, 45, 46, 47, 48, 49, 50,  
                   51}; 
       
        shuffle(a, 52); 
       
        // Imprimir todos los elementos barajados de las cartas 
        for (int i = 0; i < 52; i ++) 
           System.out.print(a+" "); 
          
    } 
} 
// This code is contributed by Arnav Kr. Mandal
# ProyectojavaBaraja
