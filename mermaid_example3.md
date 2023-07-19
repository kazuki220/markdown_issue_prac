## Class diagram

```
---  
title: Animal example　#タイトル：動物の例  
---  
classDiagram  #クラス図  
    note "From Duck till Zebra"　#これは注釈で、アヒル（Duck）、シマウマ（Zebra）に関するものです。  
    Animal <|-- Duck　#これは、動物クラスがアヒルクラスを継承していることを示しています。  
    note for Duck "can fly\ncan swim\ncan dive\ncan help in debugging"　#この注釈は、アヒルクラスが持つ特性や機能についての補足情報を提供しています。中身としては、アヒルは一般的に飛ぶことができ、水中で泳ぐことができ、ダイビングもできるという特徴が書かれています。  
    Animal <|-- Fish　#これは、動物クラスが魚クラスを継承していることを示しています。
    Animal <|-- Zebra　#これは、動物クラスがシマウマクラスを継承していることを示しています。  
    Animal : +int age　#動物クラスが年齢という公開の整数型を持っていることを示しています。  
    Animal : +String gender　#動物クラスが性別という公開の文字列型を持っていることを示しています。  
    Animal: +isMammal()　#動物クラスにある動物が哺乳類であるかどうかを判定するためのisMammal()という公開メソッドを持っていることを示しています。
    Animal: +mate()　#動物クラスにある動物が繁殖を行うためのmate()という公開メソッドを持っていることを示しています。  
    class Duck{　#アヒルクラス  
        +String beakColor　#アヒルのくちばしの色を表すbeakColorという公開の文字列型を示しています。  
        +swim()　#アヒルが泳ぐアクションを実行するためのswim()という公開メソッドを示しています。  
        +quack()　#アヒルが鳴くアクションを実行するためのquack()という公開メソッドを示しています。  
    }  
    class Fish{　#魚クラス
        -int sizeInFeet　#魚のサイズ（フィート単位）を表すsizeInFeetというプライベートの整数型を示しています。  
        -canEat()　#魚が餌を食べることができるかどうかを表すcanEat()というプライベートメソッドを示しています。  
    }  
    class Zebra{　#シマウマクラス
        +bool is_wild　#シマウマが野生かどうかを表すis_wildという公開のブール型を示しています。  
        +run()　#シマウマが走るアクションを実行するためのrunという公開メソッドを示しています。  
    }  
```

参考（ https://mermaid.js.org/intro/ ）