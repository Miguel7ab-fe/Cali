import javax.swing.JOptionPane;
public class Calificacion {
     public static void main(String args[]){
       byte x,y;
       byte cal[][] = new byte [6][4];
       String materias[]={"MatemDis","FundaInv","FundaPro","CalcDife","Quimica  ","DesaSust"};
       String encabezado[]={"Asignatura","U1","U2","U3","U4"};
       
       for(x=0;x<5;x++){
           System.out.print(encabezado[x] + "\t");
       }
       System.out.println();
       for(x=0;x<6;x++){
           System.out.print(materias[x] + "\t");
           for(y=0;y<4;y++){
               cal[x][y]=Byte.parseByte(JOptionPane.showInputDialog("Ingresa calificacion de la "
                       +encabezado[y+1]+ "De la materia " + materias[x]));
               System.out.print(cal[x][y] + "\t");
           }
           System.out.println();
       }
   } 
    
}
