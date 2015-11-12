# Aula prática, 12/11 (Quinta feira)

## Tópicos abordados
 - Classes abstratas, interfaces, tipos genéricos e *collections* (aula [01](../01_slides-java-abstract-2015b.pdf));
 - GUI com Java, [AWT](http://docs.oracle.com/javase/8/docs/api/java/awt/package-summary.html), [SWING](http://docs.oracle.com/javase/8/docs/api/javax/swing/package-summary.html), MVC.

## Material extra
 - [Tutoriais da Oracle](http://docs.oracle.com/javase/tutorial/uiswing/examples/components/index.html) para construção de interfaces gráficas em Java com SWING;

## Parte 1
 1. O programa [SemIDE.java](SemIDE.java) ilustra o uso do pacote [javax.swing](http://docs.oracle.com/javase/8/docs/api/javax/swing/package-summary.html) para criação de uma interface gráfica bastante simples. Compile e execute este programa, busque entender seu funcionamento. 
 2. Modifique o programa para que a contagem do contador seja apresentada juntamente ao título.
 3. Modifique o programa, adicionando um segundo botão na janela. 
 4. Observe o comportamento do programa. Para evitar a sobreposição entre componentes atualize o método `criaComponentes` de `SemIDE`, adicionando um `GridLayout` como gerenciador de layout.
 5. Adicione um `ActionListener` ao segundo botão e faça-o decrementar o contador `contagemCliques`. Lembre-se de atualizar a view!

