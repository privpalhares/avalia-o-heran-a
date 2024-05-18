class Main {
    public static void main(String[] args) {
        Funcionario F = new Funcionario("Marciano", 45, 150.0, 100);
        Lider L = new Lider("Mariane", 15, 150.0, 100);
        Gerente G = new Gerente("Pedro", 89, 150.0, 100);

        System.out.println(F.getNome() + ": " + F.calcularSalario());
        System.out.println(L.getNome() + ": " + L.calcularSalario());
        System.out.println(G.getNome() + ": " + G.calcularSalario());
    }
}

class Funcionario {
    private String nome;
    private int hora;
    private double calcHora;

    public Funcionario(String nome, int hora, double calcHora) {
        this.nome = nome;
        this.hora = hora;
        this.calcHora = calcHora;
    }

    public String getNome() {
        return nome;
    }

    public double calcularSalario() {
        return hora * calcHora;
    }
}

class Lider extends Funcionario {
    public Lider(String nome, int hora, double calcHora) {
        super(nome, hora, calcHora);
    }

    @Override
    public double calcularSalario() {
        return super.calcularSalario() * 1.02;
    }
}

class Gerente extends Funcionario {
    public Gerente(String nome, int hora, double calcHora) {
        super(nome, hora, calcHora);
    }

    @Override
    public double calcularSalario() {
        return super.calcularSalario() * 1.05;
    }
}
--------------------------------------------------
public class Main {
    public static void main(String[] args) {
        Retangulo retanguloSimples = new RetanguloSimples("normal");
        retanguloNormal.desenhar();

        Retangulo retanguloRedondo = new RetanguloRedondo("redondo");
        retanguloRedondo.desenhar();
    }
}
abstract class Retangulo {
    protected String texto;

    public Retangulo(String texto){
        this.texto = texto;
    }
    public abstract void desenhar();
}

public class RetanguloSimples implements Retangulo {
    private int largura;
    private int altura;
    private String texto;

    public RetanguloSimples(int largura, int altura, String texto) {
        this.largura = largura;
        this.altura = altura;
        this.texto = texto;
    }

public void representação() {
        System.out.println("──────────────");
        for (int i = 0; i < altura; i++) {
            System.out.println("│" normal "              │");
        }
        System.out.println("──────────────");
        System.out.println(texto);
    }
}

class RetanguloArredondado implements Retangulo {
    private int largura;
    private int altura;
    private String texto;

    public RetanguloArredondado(int largura, int altura, String texto) {
        this.largura = largura;
        this.altura = altura;
        this.texto = texto;
    }

    public void desenhar() {
        System.out.println("╭──────────────╮");
        for (int i = 0; i < altura; i++) {
            System.out.println("│" + "              │");
        }
        System.out.println("╰──────────────╯");
        System.out.println(texto);
    }
}

