# Aula prática, 12/11 (Quinta feira)

## Tópicos abordados
 - Classes abstratas, interfaces, tipos genéricos e *collections* (aula [01](../01_slides-java-abstract-2015b.pdf));
 - GUI com Java, [AWT](http://docs.oracle.com/javase/8/docs/api/java/awt/package-summary.html), [SWING](http://docs.oracle.com/javase/8/docs/api/javax/swing/package-summary.html), MVC. (aula [02](../02_slides-java-gui-2015b.pdf)).

## Material extra
 - [Tutoriais da Oracle](http://docs.oracle.com/javase/tutorial/uiswing/examples/components/index.html) para construção de interfaces gráficas em Java com SWING;

## Parte 1
 1. O programa [SemIDE.java](SemIDE.java) ilustra o uso do pacote [javax.swing](http://docs.oracle.com/javase/8/docs/api/javax/swing/package-summary.html) para criação de uma interface gráfica bastante simples. Compile e execute este programa, busque entender seu funcionamento.
 2. Modifique o programa para que a contagem do contador seja apresentada juntamente ao título do `JFrame`.
 3. Modifique o programa, adicionando um segundo botão na janela. 
 4. Observe o comportamento do programa. Para evitar a sobreposição entre componentes atualize o método `criaComponentes` de `SemIDE`, adicionando um `GridLayout` como gerenciador de layout.
 5. Adicione um `ActionListener` ao segundo botão e faça-o decrementar o contador `contagemCliques`. Lembre-se de atualizar a view!

## Parte 2
 1. Baixe o arquivo [JavaGUI.zip](JavaGUI.zip) que contém o projeto NetBeans usado neste exercício. Descompacte o projeto e abra-o na IDE.
 2. Observe o código fonte do projeto e veja que alguns dos eventos estão preparados para receber o código (marcados com "TODO: COMPLETE-ME") e outros não.
 3. Vincule ao evento do botão "Retornar ao padrão" a ação de restaurar os componente da interface gráfica a seus valores iniciais. Note que a JTextArea deverá ter seu conteúdo apagado. O propósito dessa operação é "reiniciar" a interface gráfica.
 4. Vincule um evento ao botão "Label" que efetue a substituição do texto do botão pelo texto informado na JTextBox.
 5. Vincule um evento que ao clicar no botão "Desabilita", desabilite todos os outros botões exceto o "Retornar ao Padrão" e "Habilita".
 6. Vincule um evento que ao clicar no botão "Habilita", habilite os botões desabilitados no passo 5.
 7. Vincule um evento que ao clicar no botão "Insere", adiciona na JTextArea o conteúdo da JTextBox.
 8. Altere um dos botões para mostrar um ícone/imagem (a sua escolha) ao invés de seu título.
 9. Altere os eventos dos botões para que ao clicá-lo, sejam registrados na JTextBox, a hora (pode ser de `System.currentTimeMillis()`) e o botão apertado.


## Parte 3 (extra): Exercício com interfaces
 1. Baixe o arquivo [ExercicioComparator.zip](ExercicioComparator.zip) que contém o projeto NetBeans usado neste exercício.
 2. Estude a classe `exercicio_comparator.comparators.ComparatorPlaca`, responsável por comparar dois objetos `Veiculo`. Veja seu método `compare()` e o comentário presente no código.
 3. Implemente duas classes que estendem `Comparator`:
    - Uma delas deve comparar dois veículos pela marca;
    - A outra deve comparar pelo preço.
 4. Complete o programa `exercicio_comparator.ExercicioComparator`. Veja as marcações `TODO: COMPLETE-ME` presentes no código.
