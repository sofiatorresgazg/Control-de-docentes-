# Control-de-docentes-
public class Profesor {

    private String nombre;
    private int edad;
    private String email;

    // Constructor vacío
    public Profesor() {
    }

    // Constructor con parámetros
    public Profesor(String nombre, int edad, String email) {
        this.setNombre(nombre);
        this.setEdad(edad);
        this.setEmail(email);
    }

    // Getters
    public String getNombre() {
        return nombre;
    }

    public int getEdad() {
        return edad;
    }

    public String getEmail() {
        return email;
    }

    // Setters con validaciones básicas
    public void setNombre(String nombre) {
        if (nombre == null || nombre.trim().isEmpty()) {
            throw new IllegalArgumentException("El nombre no puede estar vacío.");
        }
        this.nombre = nombre;
    }

    public void setEdad(int edad) {
        if (edad < 0 || edad > 120) {
            throw new IllegalArgumentException("La edad debe estar entre 0 y 120.");
        }
        this.edad = edad;
    }

    public void setEmail(String email) {
        if (!esEmailValido(email)) {
            throw new IllegalArgumentException("El email no es válido.");
        }
        this.email = email;
    }

    // Validación de email
    private boolean esEmailValido(String email) {
        if (email == null || email.length() < 5) {
            return false;
        }
        return email.contains("@") && email.contains(".");
    }

    // Métodos de interacción
    public void saludar() {
        System.out.println("Hola, soy el profesor " + this.nombre);
    }

    public void enseñar() {
        System.out.println(this.nombre + " está enseñando una clase...");
        System.out.println(this.nombre + " terminó la clase.");
    }
}

