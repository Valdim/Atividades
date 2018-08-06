import java.util.Scanner;
public class Dever {
    public static void main(String[]args){
       Scanner tcl = new Scanner(System.in);
       int vet[] = new int[10];
       int aux = 0;
       for(int i = 0; i < vet.length;i++){
           vet[i] = tcl.nextInt();
       }
       for(int i = 1;i < vet.length;i++){
           for(int j = 0;j < i;j++){
               if(vet[i] < vet[j]){
                   aux = vet[i];
                   vet[i] = vet[j];
                   vet[j] = aux;
                  
               }
           }
       }
       for(int i = 0;i < vet.length;i++){
           System.out.println(vet[i]);
       }
    }
}
