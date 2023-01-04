# ejercicio-tema-9-bootcamp

public class Main {
    public static void main(String[] args) {
        System.out.println("\nEjercicio Tema 9\n");
        System.out.println("---------------------------------------------\n");
        Cliente cliente=new Cliente();
        cliente.setNombre("Erik");
        cliente.setEdad(25);
        cliente.setTelefono(1166209612);
        cliente.setCredito(20000000);
        System.out.println("Nombre del cliente:" + cliente.getNombre());
        System.out.println("Telefono:" + cliente.getTelefono());
        System.out.println("Edad:" + cliente.getEdad());
        System.out.println("Credito:" + cliente.getCredito());

        System.out.println("---------------------------------------------\n");
        Trabajador trabajador=new Trabajador();
        trabajador.setNombre("Fabian");
        trabajador.setEdad(25);
        trabajador.setTelefono(1166209610);
        trabajador.setSalario(450000);
        System.out.println("Nombre del trabajador:" + trabajador.getNombre());
        System.out.println("Telefono:" + trabajador.getTelefono());
        System.out.println("Edad:" + trabajador.getEdad());
        System.out.println("Salario:" + trabajador.getSalario());
        System.out.println("---------------------------------------------\n");

    }

}

class Persona{
    private String nombre;
    private int edad, telefono;

    public String getNombre() {
        return nombre;
    }

    public void setNombre(String nombre) {
        this.nombre = nombre;
    }

    public int getEdad() {
        return edad;
    }

    public void setEdad(int edad) {
        this.edad = edad;
    }

    public int getTelefono() {
        return telefono;
    }

    public void setTelefono(int telefono) {
        this.telefono = telefono;
    }
}

final class Cliente extends Persona{
    private int credito;

    public int getCredito() {
        return credito;
    }

    public void setCredito(int credito) {
        this.credito = credito;
    }
}

final class Trabajador extends Persona{
    private int salario;

    public int getSalario() {
        return salario;
    }

    public void setSalario(int salario) {
        this.salario = salario;
    }
}
