First Contact*: lógica, procedimetos, especificação, implementação, testes
==========================================================================
Deu certo [:)](https://raw.githubusercontent.com/poo-2019-1/ava-00-procedimentos/master/yes.jpg)
Deu errado [:(](https://raw.githubusercontent.com/poo-2019-1/ava-00-procedimentos/master/no.jpg)

* * *

## Implementar usando métodos e testar segundo as especificações

#### Prazo: 2019-03-10 Peso: 0.5 pts

**Restrição: não podem ser usadas as bibliotecas do Java, por exemplo, a classe `Math`, `Scanner`, etc, inclusive os métodos de Integer, como `parseInt` ou métodos de String, EXCETO `length`, `charAt` e `equals`; Os Casos de Teste podem ser corrigidos, mas a especificação não pode ser alterada.**

### Exponenciação 0.2 pts

Implementar um método para fazer potência de inteiros.

Casos de teste:

```java
// Exponenciacao.java
// método potencia que entram dois inteiros e sai um inteiro
// potencia(int,int):int
int base = 3;
int expoente = 4;
int result = potencia(base, expoente);
System.out.println(result); // imprime 81
System.out.println(result == 81); // imprime true
// Casos de Teste:
System.out.print("potencia(3, 2) == 9 "); // 3 ao quadrado
System.out.println(potencia(3, 2) == 9); // 3 ao quadrado
System.out.print("potencia(2, 3) == 8 "); // 2 ao cubo
System.out.println(potencia(2, 3) == 8); // 2 ao cubo
// Números grandes
System.out.print("potencia(23, 6) == 148035889 ");
System.out.println(potencia(23, 6) == 148035889);
System.out.print("potencia(2, 30) == 1073741824 ");
System.out.println(potencia(2, 30) == 1073741824);
// 0.1 pts até aqui
// Casos Especiais: bases negativas
System.out.print("potencia(-2, 3) == -8 ");
System.out.println(potencia(-2, 3) == -8);
System.out.print("potencia(-2, 4) == 16 ");
System.out.println(potencia(2, 4) == 16);
// Casos não cobertos: expoente negativo
System.out.print("potencia(2, -3) == 0 ");
System.out.println(potencia(2, -3) == 0);
System.out.print("potencia(7, -2) == 0 ");
System.out.println(potencia(7, -2) == 0);
// 0.2 pts até aqui
// Adicione mais 2 Casos de Teste
```
### Rotacionar String (_rotate_) 0.2 pts

Dada uma `String` de entrada rotacioná-la em sentido horário.

Casos de Teste:

```java
// Rotacionar.java
String s1 = "worf";
String s2 = rotate(s1);
System.out.println(s1); // worf
System.out.println(s2); // fwor
System.out.println(s2.equals("fwor") == true); // true
String s3 = rotate(s2);
System.out.println(s3); // rfwo
System.out.println(s3.equals("rfwo") == true); // true
System.out.println(rotate("kira").equals("akir") == true);
System.out.println(rotate(rotate(s3)).equals("worf") == true);
// 0.1 pts até aqui
// Casos Especiais
System.out.println(rotate("").equals("") == true);
System.out.println(rotate("a").equals("a") == true);
System.out.println(rotate("aa").equals("aa") == true);
// 0.2 pts até aqui
// Adicione mais 2 Casos de Teste
```

### Desbastar String (_chop_) 0.2 pts

Implementar o método `chop`, em classe separada `Text`, que toma uma `String` de entrada e devolve outra sem o último caractere.

Casos de Teste:

```java
// Desbastar.java
String s1 = "seven of nine";
String s2 = chop(s1);
System.out.println(s1); // seven of nine
System.out.println(s2); // seven of nin
System.out.println(s2.equals("seven of nin") == true); // true
String s3 = chop(s2);
System.out.println(s3); // seven of ni
System.out.println(s3.equals("seven of ni") == true); // true
System.out.println(chop("spock").equals("spoc") == true);
// 0.1 pts até aqui
// Casos Especiais
System.out.println(chop("Q").equals("") == true);
System.out.println(chop("").equals("") == true);
System.out.println(chop(chop(chop("abc"))).equals("") == true);
// 0.2 pts até aqui
// Adicione mais 2 Casos de Teste:
```

[* First Contact](https://www.youtube.com/watch?v=2orQxtEmtjE)