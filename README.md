# first repository
alguns estudos

## Links úteis

[sintaxe basica de markdown](https://www.markdownguide.org/basic-syntax/)

[alguns comandos do git](https://www.codigofonte.com.br/artigos/top-25-comandos-do-git)

[solução de problemas para github, gitlab e git repos e rastreamento de problemas](https://cloud.ibm.com/docs/ContinuousDelivery?topic=ContinuousDelivery-troubleshoot-git&mhsrc=ibmsearch_a&mhq=github)

[livros de programação gratuitos](https://github.com/EbookFoundation/free-programming-books/blob/main/books/free-programming-books-pt_BR.md)


# introdução ao C# e .NET

## estruturas
### namespace

os namespaces são usados para organizar classes. 

.net e c# usam os namespaces para controlar as classes deles;

para usar uma classe de outro namespace, colocamos ```using``` no começo do código.

#### duas formas de acessar a classe de um namespace

colocar o nome(do namespace), seguido por ```.``` e nome da classe

ex: ```System.Console```

ou colocar o ```using``` como dito anteriormente.

### classe

uma classe pode ter campos, propriedades, métodos e eventos dentro dela, que são denominados **membros**

quando uma classe é instanciada, essa instância é chamada de *objeto*, e nesse objeto podem ser criados valores de acordo com os campos da classe. 

o valor que for criado para o objeto, não vai ser criado para classe(e a classe vai ser utilizada para criar outros objetos).

### interface

é como uma classe base que serve de molde para outras classes. 

uma classe  que implementa interface deve implementar todos os membros.

na interface, por padrão, deve ser adicionado um **I** na frente do "nome". ex.: 

```interface IAcesso
{
   void Ler();
   void Escrever();
}
interface IComprimir
{
   void Comprimir();
   void Descomprimir();
} 
```

### enum 

[declara um conjunto de constantes nomeadas que começam do 0 e aumentam de 1 em 1](https://www.devmedia.com.br/trabalhando-com-structures-e-enum-em-csharp/32259)
