## Class diagram
```
classDiagram #クラス図  
Class01 <|-- AveryLongClass : Cool　#
Class03 *-- Class04　#class03とclass04には、関連の一種である、複合の関係で表されています。  
Class05 o-- Class06　#class05とclass06には、関連の一種である、集約の関係で表されています。  
Class07 .. Class08　#class07とclass08には、双方向の関連を示す連結線で表されています。  
Class09 --> C2 : Where am i?
Class09 --* C3
Class09 --|> Class07
Class07 : equals()
Class07 : Object[] elementData
Class01 : size()
Class01 : int chimp
Class01 : int gorilla
Class08 <--> C2: Cool label
```