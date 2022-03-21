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


### debugging 

em português, depuração, é o nome dado ao processo de encontrar e remover os erros que podem acometer softwares e hardwares. O termo faz parte do processo de desenvolvimento desde o início e há quem diga que ele foi criado antes mesmo dele.


# CLI do dotnet(basics)

```dotnet --help``` fornece a documentação da interface do .net na linha de comando.

```new``` permite que criemos um projeto ou um arquivo dentro da pasta em que estamos.

```nuget``` é um gerenciador de pacotes para dotnet.

```run``` comando que builda e roda sua aplicação 

```test``` cria um projeto de teste que vai automatizar os testes da sua aplicação.

```tool``` permite que você instale e gerencie ferramentas de extensão pro dotnet.

```publish``` comando para subir o site em algo como um servidor web.

```restore``` restaura os pacotes atrelados ao nuget.

```build``` compila o código e gera uma linguagem intermediária.(dll é um código compilado em uma linguagem intermediária.)

conhecendo o C#
===============

> linguagem que teve seu início no final da década de 90 e emergiu junto ao .net,  
> elegante, orientada a objeto e fortemente tipada.  a sintaxe do C# é similar às do C, C++ e Java.

suporta os conceitos da orientação objeto como encapsulamento, herança e polimorfismo (OO)

os programas C# são executados no .net, que inclui:  

+ CLR(common language runtime)
+ conjunto unificado de bibliotecas de classes.

atualmente seu compilador é o *roslyn*.

## como funciona

> o código-fonte escrito em C# é compilado em uma linguagem intermediária(IL).  
> o código e os recursos de IL são armazenados no disco em um arquivo executável chamado *assembly*, geralmente com uma extensão ***.exe ou .dll***.

quando o programa C# é executado, o assembly é carregado no CLR

em seguiga o CLR executará a compilação *just in time*(JIT) para converter o código IL(linguagem intermediária) em instruções de máquina nativas.

o CLR também fornece outros serviços:

+ garbage collector: valida/verifica objetos em memória que não estão sendo utilizados e desaloca esses objetos da memória.
+ exception handler: recebe e controla as exceções que ocorrem de erros no nosso código.
+ resources manager: literalmente gerenciador de recursos.

além dos serviços de tempo de execução, o .net também inclui uma extensa biblioteca com milhares de classes que fornecem uma ampla variedade de funcionalidades úteis, desde entrada e saída de arquivos, manipulação de cadeias de caracteres, analise xml, etc.

***

# estrutura de programa

os principais conceitos organizacionais em C# são:

+ programas
+ namespaces
+ tipos
+ membros
+ assemblies

programas em C# consistem em um ou mais arquivos.<br> os **programas** declaram **tipos** que contém **membros** e podem ser oganizados em **namespaces**

*classes e interfaces* são exemplos de **tipos**.<br> *campos, métodos, propriedades e eventos* são exemplos de **membros**.

quando os programas C# são compilados, eles são fisicamente empacotados em ```assemblies```. <br> os assemblies geralmente tem a extensão de arquivo **.exe ou .dll** dependendo se são aplicações ou bibliotecas.
