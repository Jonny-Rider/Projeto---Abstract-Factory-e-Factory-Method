# Projeto-Abstract-Factory-e-Factory-Method

- Intenção:

Fornece uma interface para criar famílias de objetos relacionados ou dependentes sem especificar suas classes concretas.
Uma hierarquia que encapsula: muitas "plataformas" possíveis e a construção de um conjunto de "produtos".
O novo operador considerado prejudicial.

- Implementação:

-Decida se a "independência de plataforma" e os serviços de criação são a fonte atual de problemas.

-Mapeie uma matriz de "plataformas" versus "produtos".

-Defina uma interface de fábrica que consiste em um método de fábrica por produto.

-Defina uma classe derivada de fábrica para cada plataforma que encapsula todas as referências ao novo operador.

-O cliente deve retirar todas as referências ao novo e usar os métodos de fábrica para criar os objetos do produto.

- Estrutura:

O Abstract Factory define um Método de Factory por produto. Cada método de factory encapsula o novo operador e as classes de produto concretas e específicas da plataforma. Cada "plataforma" é então modelada com uma classe derivada de Factory.

![alt text](https://sourcemaking.com/files/v2/content/patterns/Abstract_Factory.png)

- Exemplo:

O objetivo do Abstract Factory é fornecer uma interface para a criação de famílias de objetos relacionados, sem especificar classes concretas. Esse padrão é encontrado no equipamento de estampagem de chapa metálica usado na fabricação de automóveis japoneses. O equipamento de estamparia é uma Abstract Factory que cria peças de carroceria. A mesma máquina é usada para estampar portas direitas, portas esquerdas, pára-lamas dianteiros direitos, pára-lamas dianteiros esquerdos, capôs, etc. para diferentes modelos de carros. Por meio do uso de rolos para troca das matrizes de estampar, as classes de concreto produzidas pelo maquinário podem ser trocadas em três minutos.

![alt text](https://sourcemaking.com/files/v2/content/patterns/Abstract_Factory_example1.png)
