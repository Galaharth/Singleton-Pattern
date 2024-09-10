# Singleton-Pattern
Singleton pattern is created to make a way that the class' instance is unique and cannot be duplicated.

O padrão Singleton serve para impedir que mais de uma instância de uma mesma classe seja criada. O padrão deve conter um construtor privado, uma instância dentro da classe e um método público e estático que contenha uma única instância. 

 

public class Singleton { 

    // Instância privada estática da classe 

    private static Singleton instancia; 

  

    // Construtor privado para evitar instanciamento externo 

    private Singleton() { 

        // Inicialização, se necessário 

    } 

  

    // Método público estático para obter a instância única 

    public static Singleton getInstancia() { 

        if (instancia == null) { 

            // Cria a instância apenas se ela não existir 

            instancia = new Singleton(); 

        } 

        return instancia; 

    } 

} 

 
