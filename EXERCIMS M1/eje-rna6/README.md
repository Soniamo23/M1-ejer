# React + TypeScript RNA

Importación de React y CSS:
Importamos React desde la biblioteca de React para poder definir componentes de React.
Importamos el archivo CSS necesario. Esto es opcional y depende de si deseas aplicar estilos al componente App.
Definición de la interfaz M:
Se define una interfaz llamada M, que especifica que cualquier propiedad de tipo cadena debe tener un valor de tipo cadena. Esta interfaz se utiliza para definir el tipo del objeto Map, que mapea las bases de ADN a las bases de ARN.
## Objeto Map:

toRna es una función que realiza la transcripción de ADN a ARN.
Toma una cadena de ADN como entrada y devuelve una cadena de ARN como salida.
Primero, verifica si la cadena de ADN contiene caracteres que no son 'A', 'C', 'G' o 'T'. Esto se hace utilizando una expresión regular (/[^ACGT]/) y el método test. Si encuentra algún carácter no válido, lanza un error.
Luego, utiliza el método replace en la cadena de ADN para reemplazar cada base de ADN con su correspondiente base de ARN utilizando el objeto Map definido anteriormente.
## Componente App:
App es un componente de React que devuelve la interfaz de usuario.
Dentro de este componente, se llama a la función toRna con una cadena de ADN de ejemplo ("GCTA") y se muestra la cadena de ADN original y la cadena de ARN resultante en la interfaz de usuario.
Se utiliza JSX para definir la estructura del componente. JSX es una extensión de sintaxis de JavaScript que permite escribir código similar a HTML dentro de componentes de React.
##Exportación de App:
El componente App se exporta para que pueda ser importado y utilizado en otros archivos de tu aplicación.
