# Sustentacion-practica-1.Luisa
Solución del ejercicio enviado por el profesor para realizar la sustentación #1

public class Practica{
    public static void main(String[] args) {
        
        practica1 datosprod = new practica1("Aguardiente",25,11500);  
        
        //Mientras la opcin elegida sea 0, preguntamos al usuario
		while(select != 0){
				System.out.println("Elige opcin:\n1.- Agregar" +
						"\n2.- Buscar\n" +
						"3.- Eliminar\n" +
						"4.- Mostrar\n" +
                        "5.- venta\n" +
                        "6.- Ganancia\n" +
						"0.- Salir");
				
	//Recoger una variable por consola
	select = Integer.parseInt(scanner.nextLine());

		switch(select){
		case 1:		
            datosprod.Agr();
        break;
        
        case 2:
            datosprod.bus();
       break;
                
        case 3:
            datosprod.eli();
        break;
                
        case 4:
            datosprod.mos();        
        break;
        
        case 5:
            datosprod.ven();       
        break;
        
        case 6:
            datosprod.gan();        
        break;
        
        default:
                select=0;
                
        
		}
		
           
    }    
}


public class practica1 {
    
    //atributos
    private String nombre;
    private int cantidad;
    private int valor;
    
    public practica1(String nombre, int cantidad, int valor) {
        this.nombre = nombre;
        this.cantidad = cantidad;
        this.valor = valor;
    }
    public void agr(){
      Scanner lector = new Scanner(System.in);
        System.out.println("Digite el nombre: ");
        nombre=lector.next();
        System.out.println("Digite la cantidad: ");
        cantidad = lector.nextInt(); 
        System.out.println("Digite el valor: ");
        valor = lector.nextInt(); 
}
    public void bus(){
    System.out.println("El nombre es: "+nombre);
    System.out.println("La cantidad es: "+cantidad);
    System.out.println("El valor es: "+valor);
    }
    public void eli(){
        
    }
    public void mos(){
    }
    public void ven(){
    }
    public void gan(){
    }
    
}
