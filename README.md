package tda;

public class Principal {

    public static void main(String[] args) {
     CalculoAngulos obj = new CalculoAngulos();
     
     
     obj.AnguloCentral();
     obj.AnguloInterior();
     obj.AnguloExterior();
    }
    
}



package tda;


public class CalculoAngulos {
    
    // n= numero de lados
    int n = 5;
public void AnguloCentral (){
    
int a;
double r; 

a = 360/n;
r = (2 * Math.PI)/n;

System.out.println("Angulo Central" ); 
System.out.println("En Grados Sexagesimales " + a ); 
System.out.println("En Radianes " + r);
}

public void AnguloInterior (){
int b;
double r;

b = 180*(n-2);
r = Math.PI * (n-2)/n;

System.out.println("\n Angulo Interior" );
System.out.println("En Grados Sexagesimales " + b ); 
System.out.println("En Radianes " + r);

}

public void AnguloExterior (){
int r;
double ra;

r = 360/n;
ra = (Math.PI *2)/n;

System.out.println("\n Angulo Exterior" );
System.out.println("En Grados Sexagesimales " + r ); 
System.out.println("En Radianes " + ra);

}
   }
