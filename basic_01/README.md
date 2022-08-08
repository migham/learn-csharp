# Partes de un programa en C#
Cuando nosotros creamos un proyecto en C#, el SDK nos crea por defecto un esqueleto para que podamos empezar a trabajar en nuestro código.



## using

La primera sección que nos crea el SDK es la seccion using, esta sentencias nos sirve para importar otros _namespace_ tanto del mismo sistema como de 3eros... pero.. que c#$%& es un namespace?

Un namespace se lo puede tomar como un espacio lógico donde nosotros podemos tener diferentes recursos, tales como clases, enumeraciones, estructuras, etc.. 

Nosotros podemos crear nuestros propios namespace, pero a su vez Microsoft ya ha creado sus propios namespace y dentro del Runtime existen varios namespace que nosotros podemos utilizar en diferentes aplicaciones que asi lo requieran.

Por defecto el SDK nos añade el namespace `System` 

## namespace
Al crear un proyecto desde cero, automaticamente se crea un namespace dentro de nuestro Program.cs con el nombre de nuestro proyecto, en nuestro caso `basic_01`. Algo que podemos hacer, es renombrar el namespace a nuestro gusto sin problema alguno. 

La idea del namespace es justamente poder organizar varios archivos del proyecto bajo un orden lógico. Asi que sí, podemos tener varios archivos con el mismo namespace. el SDK al momento de tener que compilar, va a poder relacionar entre si los documentos que contengan el mismo namespace y mi programa, podrá utilizar todo aquello que se encuentre dentro del namespace sin mayor problema.

al momento de declarar el namespace, este es continuado por dos llaves, una de apertura y otra de cierre.

```csharp
namespace basic_01
{
	// codigo por aqui del namespace
}
```

Esto se conoce como bloque de código y nos está indicando un área en particular, entonces todo lo que se encuentre entre estas dos llaves, pertenecerá al namespace `basic_01` aunque el namespace se puede declarar en varios documentos.

## class
C# es un lenguaje orientado extrictamente a objetos, lo que significa que realmente todo lo que aparezca en el lenguaje, es un objeto. Aunque de momento me me centraré en programación estructural, es mi plena intención abordar la programación orientada a objeto. Aclarado esto, hay que decir que al crear un nuevo proyecto en C#, el SDK creará una clase para nosotros, por defecto, esta clase se llamará Program. Posteriormente, cuando llevemos a cabo la compilación, se creará un objeto del tipo Program, el cual, va a ser llamado por el SO para poder ejecutar el programa.

## Main
Todo programa escrito en C# va a contener una función _Main()_ esto es sumamente importante, ya que será siempre nuestro punto de inicio del programa. Esta función es creada automáticamente cuando creamos cualquier proyecto en C#