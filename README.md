
<img src="banner.png" height="200px" width="900px"  />

# Apuntes de JavaScript

Una variable decladara en CONST ?se puede puede modicar sus valores
en... objetos y arreglos ...

Un arreglo puede tener objetos ? si

diferencia en tre foreach y map ? es que map crea un nuevo arreglo

diferencia de freeze y seal es q el seal se puede modificar pero no eliminar

freeze no se puede hacer nada ni eliminar ni modificar

funcion declaradas y funcion Expresion diferencia es q la expresion la la lee si declaras antes de la funcion
encambio la declarada lee si esta primera la declaracion o al ultimo

#### ¿Que diferencia hay entre function y arrow function ?

- El arrow busca globalmente y fuction dentro de la function

#### ¿ Como eliminas un duplicado de una array ?

Elimino con set

#### Busca dentro del objeto y no afuera sino lleva this. buscara afuea otro const

- THIS

```javascript
const n = {
    nombre = rafael

	mostrarinfo function (){
		console.log('el nombre es ${this.nombre}')

}
n.mostrarinfo();   // consola el nombre es rafael
```

- this
- object constructor

function producto (nombre , precio){
this.nombre = nombre;
this.precio=precio;
this.disponible = true;
}
const producto2 = new producto ('monitor 24' , 5000);
console.log(producto2);

consola nomre : monito 24 , precio: 5000

/////////////////////////////////////////////////////

console.log(objeto.keys(producto)); izquida muestra " nombre :"
console.log(objeto.values(producto)); derecha muestra "rafael"
console.log(objeto.entries(producto)); muestra en par nombre: rafael
///////////////////////////////////////////////////
const meses = [junio,julio]
meses.push('octubre');// agrega
console.table(meses);
console.log(meses.length);

for (let i= o ; i<meses.length; i++){
console.log( meses[i]); // se veran todos
}
/////////////////////////////////////////////////////////////////
arrow function

funtion () = a () =>

const aprendiendo = function (){
console.log('aprendiendo java');
}
aprendiendo ();
............................................
const aprendiendo2= ()=>'aprendiendo java';
}
console.log (aprendiendo2 ()); // aprendiendo java
............................................
const datos= (nombre)=>'el se llama ${nombre}';
//2- aqui inserta a (nombre= rafael) 3- luego lo lleva a aqui${rafael}

console.log (datos(rafael)); // 1- pone el nombre // El se llama rafael
.............................................

const carrito = [
{ nombre: 'Monitor 20 Pulgadas', precio: 500},
{ nombre: 'Televisión 50 Pulgadas', precio: 700},
{ nombre: 'Tablet ', precio: 300},
{ nombre: 'Audifonos', precio: 200},
{ nombre: 'Teclado', precio: 50},
{ nombre: 'Celular', precio: 500},
]

// map crea un nuevo arreglo y foreach no // crea const para q se almacencen hay // para ser llamado por consola
// "PRODUCTO" es una nueva variable creada por asi decirlo para la los datos dentro de la ARAY

const nuevoArray = carrito.map( producto => `Articulo: ${ producto.nombre } Precio: $ producto.precio} `)

carrito.forEach( producto => console.log( `Articulo: ${ producto.nombre } Precio: $ producto.precio} `));

console.log(nuevoArray);

////////////////////////////// ANTES ARRIBA ARROW ///////////////////////
const nuevoArray = carrito.map( function(producto) {
return `Articulo: ${ producto.nombre } Precio: $ producto.precio} `;
})

const nuevoArray2 = carrito.forEach( function(producto) {
return `Articulo: ${ producto.nombre } Precio: $ producto.precio} `;
})

/////////////////////////////////////////////////////////////////////////
=== = si o si es igual
== = puede ser igual pero no tan igual
!== = menos o diferente a tal

> = mayor a meno
> < = menor a mayor
> if = es --> ?
> else = es -->;
> let = 0 ; // += va sumando y lo almacena en el LED
> reduce = + , 0 hace q se sume pero con inicializador numero q yo quiera q inicie pongamosle 2000 y

    	 no va usar led  como usa arriva con LED = 0 no usara
    	definira como un carrito.reduce(total.producto) total + producto.precio,0

break = detiene todo
continue = sigue
function = ()=>
this. = va dentro de de su raid o objetos busca dentro no afuera
for = recorre y tiene su funcion
while = si no cumple la funcion no recorre
do while = recorre una vez y luego sino cumple la funcion no recorre
foreach = no crea una nueva raid
map = crea una nueva raid
for of = interactua con raid y busca elementos no indices
for in = busca indices dentro de un objeto y en arraid indices // pero no vuelve nada si no encuentra

Every = es raro, ya que TODOS los elementos del arreglo deberán cumplir esa condición.. // false // version del &&
some = busca 1 vedadero y falso si estan o no dentro de objetos 1 debecumplir la condicion // true // version del || ord

includes = busca vedadero y falso si estan o no dentro de ARRAY
findIndex = para lo q no encuentra tirar ""-1""
filter = trae todo y crea una nueva raid con su nueva conducion d operadores
find = llama una sola vez cuando se cumple la condicion y si hay mas de 2 solo trae el primero

concat. = une arrays
rest operator o spread operator "..." = ...meses1,...meses2,mes,'otromes' y une las array pero tienes q poner ordenadamente
'otromes' se agrega haci y si lepones ... armara nuevas array con cada letra// no hacer
para meter un nuevo producto o "mes12" se pone sin comillas y sin ... puntitos...
se crea una nueva constante y como objeto para meterlo adentro de la ray mes

dom = elementos de tu pagina html que te permite seleccionarlos y modificarlos para mostrar por pantalla tu pagina web
const heading = document.querySelector('h1');// asi nos crearemos la clase y nos dirigiremos como queremos
getElementsByClassName = busca clases retorna 1 y el primero que encuentre
getElementById = busca ID y retorna 1 y el primero que encuentre
querySelector = busca ID Y CLASES y retorna el primero que encuentre y usa sentencia de CSS para encontrarlos ID se seleciona """"#"""""
querySelectorAll = busca id y clases y retorna TODOS auque traer VARIAS ID sea malas practicas ID se seleciona """"#"""""

imagen.src = 'img/hacer2.jpg'; = para cambiar imagenes
console.log(encabezado.innerText); // = si le ponemos a ese elemento visibility: hidden; en el CSS,
console.log(encabezado.textContent); // = entra al texto y modifica
console.log(encabezado.innerHTML); // = se trae el html

console.log(heading.style);//= cambiar el color
// heading.style.backgroundColor = 'red'; // Nota como las propiedades que le puedes pasar, son similares a las de CSS, con la diferencia de que el guion se elimina y la segunda palabra su primer letra es mayuscula.
// heading.style.textTransform = 'uppercase';
// heading.style.fontFamily = 'Arial';

console.log(card.classList); //= Classlist nos permitirá listar las classes
card.classList.add('nueva-clase'); //= te permitirá añadir una clase.. // si deseas añadir múltiples classes debes agregar una coma en cada una
card.classList.remove('card'); // = de la misma forma si deseas remover múltiples classes tendrías que hacerlo agregando una coma

-----------TRAVERSING THE DOM--------
console.log(navegacion.childNodes); //= La diferencia es que childNodes te va a mostrar hasta los espacios en blanco, del ""html""
console.log(navegacion.children) //=children te muestra solo los elementos... del ""html""

console.log(card.children);
console.log(card.children[1]);//= Si quieres acceder a ese div con la clase de info puedes colocar...
console.log(card.children[1].children[1]);//= Si quieres accedera los elementos hijos de ese info... recuerda puedes anidar las propiedades.
console.log(card.children[1].children[1].textContent);//= Acceder al titulo
card.children[1].children[1].textContent = 'Cambiando el Texto con traversing...'//= Modificar ese titulo con un traversing
// Intenta cambiar el texto que dice concierto por algo más siguiendo esta sintaxis de ir navegando por el DOM...

// Cambiar la imagen...
console.log(card.children[0].src);
card.children[0].src = 'img/hacer2.jpg';

console.log(navegacion.firstChild)//= Si desesa acceder al primero
console.log(navegacion.firstElementChild);//= su deceas acceder al ultimo
navegacion.firstElementChild.textContent = 'Nuevo Enlace...'//= Cambiar el primer texto...

console.log(enlace.parentElement.parentElement)//= También puedes ir al padre del padre... y de hijo a padre

console.log(enlace.nextElementSibling); //= siguiente si esta en el mismo nivel esto se llama TRAVERSING
console.log(enlace.nextElementSibling.nextElementSibling); //= pasara 2 veces el siguiente

//= También hay una forma de ir digamos en la otra dirección... VAMOS A la posicion 4 y esto nos dirigira al 3
## console.log(ultimoCard.previousElementSibling);

primerEnlace.remove(); = REMUEVE el enlace selecionado

const borrar = navegacion.children[2]
navegacion.removeChild(borrar); //= borra con const y asignacion de posicion

APPENDCHILD""INSERTBEFORE
navegacion.appendChild(enlace); // APPENDCHILD"" = es como crear nuevo hijo a NAVEGACION del menu por ejemplo y su nuevo hijo sera enlace
navegacion.insertBefore(enlace, navegacion.children[1]); // INSERTBEFORE = colocar dentro del NAVEGACION la posicion que quiero poner mi nuevo ENLACEs

CREATEELEMENT
const enlace = document.createElement('A'); // si vamos a crear una etiqueta o generando archivos cosas d HTML

enlace.href = '/nuevo-enlace'; // añadiendo HREF
enlace.target = '\_blank' //\_blank : Carga la URL en un nuevo contexto de navegación
enlace.classList.add('enlace'); // agregando nueva clase
enlace.setAttribute('data-enlace', 'nuevo-enlace') // atributos de html
enlace.onclick = miFuncion; // crear una funcion al dar click
const navegacion = document.querySelector('.navegacion');
// console.log(navegacion.children); // vemos la posiciones
//navegacion.appendChild(enlace); // APPENDCHILD es como crear nuevo hijo a NAVEGACION del menu por ejemplo y su nuevo hijo sera enlace
navegacion.insertBefore(enlace, navegacion.children[1]); // colocar dentro del NAVEGACION la posicion que quiero poner mi nuevo ENLACEs
/_function miFuntion(){
alert('diste click') // hago mi funcion y llamo cuando den click
}_/

ADDEVENTLISTENER
btnFlotante.addEventListener('click', mostrarOcultarFooter); // cuando de click hacer funcion o evento o agregar despues de la coma va , funcion
CONTAINS
if( footer.classList.contains('activo') ) { // Constaind busca si es que esta dentro de la clase CSS activo SINO ELSE AGREGA el ACTIVO y cuando vuelva a recorrer ya esta activo aqui y muestra recien el cuadro

DOMContentLoaded' = espera q todo cargue y luego muestra ..

# TECLADO
* keydown - cuando presionas una tecla
* keyup - Cuando sueltas la tecla...
* blur - cuando sales del input - ideal para validación...
* También hay eventos para cortar copiar y pegar
# 
*  cut cuando cortan
* copy
*  paste cuando pegas algo
* input - cuando se ejecutan todas las que aquí se muestran...
* incluyendo cortar, pegar y copiar menos el blur
* e = a o leer evento

# MAUSE
* mousedown - cuando presionamos
* click - similar, de hecho es probablemente el más utilizado..
* dbclick - doble click como cuando quieres abrir un archivo
* mouseup - al soltar
* mauseenter - cuando pasas sobre el
* mauseout -cuando sales sobre el

# SUBMIT
Es como cuando alguien preciona el boton o input que tiene el SUBMIT

E.PREVENTDEFAULT()
```javascript
e.preventDefault(); // PreventDefault es evitar que el navegador realice la acción por default, en este caso ir al action.

    //  e.preventDefault();  previene la accion que tenia q hacer y le damos una nueva accion nosotros o lo q requerimos.

    // Usualmente utilizaras preventDefault para validar el formulario antes de enviarlo a un servidor.

    // Crear consultas Ajax entre otras cosas o api antes de ir al enlace predestinado.

e.target.method //saber que metodo usa si usa POST.
e.target.action // que accion hace o dnde dirije ese enlace.
```


# SCROLL
**window.scrollY**: cuantos pixeles hay de arriba y ir bajando

#### GETBOUNDINGCLIENTERECT
```javascript
.getBoundingClientRect();
```
* Este método te da el tamaño de un elemento y su ubicación respecto a la ubicación actual..en movimiento de html de arriba para abajo

# ONCLICK funcion
```javascript
parrafo3.onclick = nuevaFuncion(1); // nuevo click para dar una funcion
```


```javascript
function nuevaFuncion(id) { // CUANDO A SIDO DADO UN CLICK mostrar id
console.log('click..', id)
```


# LOCAL STORAGE
* **Local Storage** solo soporta strings, no soporta arrays ni objetos pero puedes almacenarlos convirtiendolos a string..

# PROTOTYPE
* **Prototype** = es como datos dentros de objetos para ser usado por metodos con funciones .. por que con arrow no puede solo se usa local mente no globalmente

**herencia** = de datos para otros prototypes usando create

# CLASES
**clases** = es casi igual que prototype solo que se diferencia en herencia para heredar usan la palabra "extends classObjeto anterior"
y para agregar usan 

```javascript
const juan = new cliente ('juan' , 400);

class Empresa extedes Cliente {

}
```


en herencia = usa SUPER() para ir al constructor padre.

/////////////////////////////////////////////////////////////////////
en un for loop como indetificas los pares y impares?
hacer el for (led i = 0 ; i <= 20 ; i++){
si (i % 2 ===0){
mostrar numero ${i}es par
}else {
mostrar el numero ${i} es impar
}
}

SCROLL
window.scrollY = cuantos pixeles hay de arriba y ir bajando

/////////////////////////////////////////////
como detener la array en el numero 5 si t doy 10 numeros ? // y como muestro a numero 5 en letras

for (let i = 0 ; i <= 20 ; i++){
si (i===5){
mostrar ('este es el 5'); //mostrar ('este es el CINCO');
break;
}
console ('numero : es {i}
}

///////////////////////////////////////////////
Y en que casos puedes utilizar el continue??
const carrito = [
{ nombre: 'Monitor 20 Pulgadas', precio: 500},
{ nombre: 'Televisión 50 Pulgadas', precio: 700},
{ nombre: 'Tablet ', precio: 300, descuento: true},
{ nombre: 'Audifonos', precio: 200},
{ nombre: 'Teclado', precio: 50, descuento: true},
{ nombre: 'Celular', precio: 500},
]

for(let i = 0; i <= 10; i++) {
if(carrito[i].descuento) { // ve si tiene TRUE en descuento si esverdad muestra tiene descuento
console.log(`El articulo ${carrito[i].nombre} Tiene descuento... `);
continue;
}
console.log(carrito[i].nombre); // llama el resultado q no tienen descuento

}

/////////////////////////////////////////////////////////////////////////////////
/ Fizz Buzz...
mostrar numero del 0 al 100
// 3 6 9 12 15 ... FIZZ
// 5 10 15 20 25 ... BUZZ
// 15 30 45 ... Fizz Buzz

for(let i = 1; i < 100; i++ ) {
if(i % 15 === 0) {
console.log(`${i} FIZZ BUZZ`)
} else if(i % 3 === 0) {
console.log(`${i} fizz`);
} else if ( i % 5 === 0 ) {
console.log(`${i} buzz`)
}
}
////////////////////////////////////////////////////////////////////////////////////

// Otro iterador muy común es el while loop, este se ejecuta mientras una condición sea verdadera..

let i = 100;
while (i < 10) { // condicion como no es menor el let es 100 entoces no seguira ejecutando no mostrara nada

    // Bloque de código...
    console.log(`Numero: ${i}`);



    i++; // incremento

}
//////////////////////////////////////////////////////////////////////////////////
// Veamos otro iterador que es muy común en otros lenguajes y también en javascript, es el do while...

// a diferencia del for y del while, el do while se ejecuta al menos una vez, y después verifica si la condición se cumple...

// Do While va a correr al menos una vez.
let i = 0; // probar con 1000

do {
console.log(`Numero: ${i}`)
i++;
} while( i < 10 );

// Ahora, lo que hace diferente a un while de un for o un do while, es que al menos se va a ejecutar una vez aunque la condición no se cumpla...

/////////////////////////////////////////////////////////////////////////////////////
* Bueno veamos otros iteradores que existen en JavaScript, previamente ya habiamos visto forEach y Map, vamos a verlos en este video y sus diferencias...

```javascript
let pendientes = ['Tarea', 'Comer', 'Proyecto', 'Estudiar JavaScript'];
```


* Recorrer por un Foreach
```javascript
pendientes.forEach( (pendiente, index) => {
console.log(`${index} : ${pendiente}`);
});
```

*  Recuerda que como es una sola linea, la llave es opcional...

* Recorrer arreglo de objetos
```javascript
const carrito = [
{id: 1, producto: 'Libro' },
{id: 2, producto: 'Camisa'},
{id: 3, producto: 'Disco'}
];

carrito.forEach( producto => {
console.log(`Agregaste ${producto}`);
});
```
// Lo mismo aplica para los maps, la sintaxis es la misma, solo recuerda, el map te crea un nuevo arreglo,
si solo deseas recorrer los elementos utiliza el Foreach, si requieres crear un nuevo arreglo, sin duda el map sera mejor...
//////////////////////////////////////////////////////////////////////////////////////////////
// En este video veremos for of...

// For of no es como un for tradicional que ejecuta una pieza de código mientras una condición sea verdadera,
este ejecuta mientras haya elementos por iterrar como puede ser un arreglo y otros llamados Maps y Sets que veremos más adelante...

```javascript
let pendientes = ['Tarea', 'Comer', 'Proyecto', 'Estudiar JavaScript'];

for (let pendiente of pendientes) {
console.log(pendiente);
}
```


*  Sin duda una forma más sencilla que un foreach y un for no?

```javascript
const carrito = [
    {id: 1, producto: 'Libro' },
    {id: 2, producto: 'Camisa'},
    {id: 3, producto: 'Disco'}
];
```

```javascript
for (let producto of carrito) {
    console.log(producto.producto);
    // va a traer lo q es LIBRO camisa y disco por q OF
    //va por lo q esta dentro en una array tambien iria por lo q esta adentro no lo indice
}
```


```javascript
let automovil = {
    modelo: 'Camaro',
    motor: '6.0',
    anio: '1969',
    marca: 'Chevrolet'
}
for(let auto in automovil) {
    console.log(`${auto} : ${automovil[auto]}`);
}
```

* aqui vemos q los indice son modelo , motor, anio,marca,
IN va por el indice en un ARRAY iria por 1 . 2. 3 
* tambien llamados como OBJETOS q son estos

# """"""""" Some """""""""""""""""""""

```javascript
const carrito = [
    { nombre: 'Monitor 20 Pulgadas', precio: 500},
    { nombre: 'Televisión 50 Pulgadas', precio: 700},
    { nombre: 'Tablet', precio: 300},
    { nombre: 'Audifonos', precio: 200},
    { nombre: 'Teclado', precio: 50},
    { nombre: 'Celular', precio: 500},
    { nombre: 'Bocinas', precio: 300},
    { nombre: 'Laptop', precio: 800},
];
```


* En el caso de un arreglo de objetos... .includes no es la mejor opción, podrías utilizar uno llamado .some
> forma nueva para OBJETOS

```javascript
const existe = carrito.some( producto => producto.nombre === 'Celular' );
console.log(existe);
```



# Includes
##### Forma nueva
*  O también podrías utilizar el Array Method de .includes
* Cambiar a Diciembre... confirma dentro de una array solo include funciona bien para array

```javascript
const resultado = meses.includes('Enero');

console.log(resultado);

// forma vieja
meses.forEach(mes => {
    if(mes === 'Enero') {
        console.log('Enero si existe...')
    }
})
```



# FindIndex
* te dirá el indice es decir la ubicación del elemento en el arreglo...
*  Cambiar a Diciembre, Tendremos ""-1"" eso quiere decir que no lo encontró

```javascript
const indice = meses.findIndex( mes => mes === 'Abril' );
console.log(indice);
```



* Supongamos que tenemos nuestro carrito de compras y queremos decirle al usuario cuanto es el total a pagar...

// Con un foreach lo podrías hacer asi...
```javascript
const carrito = [
    { nombre: 'Monitor 20 Pulgadas', precio: 500},
    { nombre: 'Televisión 50 Pulgadas', precio: 700},
    { nombre: 'Tablet', precio: 300},
    { nombre: 'Audifonos', precio: 200},
    { nombre: 'Teclado', precio: 50},
    { nombre: 'Celular', precio: 500},
    { nombre: 'Bocinas', precio: 300},
    { nombre: 'Laptop', precio: 800},
];

let total = 0;
carrito.forEach( producto => total += producto.precio ); 
console.log(total);
```


////////////////////////////////////////////////////
REDUCE""""""""
// Puedes ver que si bien no se ve mal, podemos tenerlo todo en una sola linea con un .reduce

// total, actual seria como un cuando creamos producto bueno este seria un deposito de numeros eso es el reduce

let resultado = carrito.reduce((total, producto) => total + producto.precio, 0); //0 es el inicio si pongo 2000 iniciara la suma despues de los 2000
console.log( resultado );

hace q se sume pero con inicializador numero q yo quiera q inicie pongamosle 2000 y
no va usar led como usa arriva con LED = 0 no usara
sino q crea su propio actual deposito de numeros
/////////////////////////////////////////////////////////////
FILTER""""""""""""
filter trae todo y crea una nueva raid con su nueva conducion d operadores
let resulta;
let resultado = carrito.filter( producto => producto.precio > 400 ); // Todos los mayores a 400 - añadir && producto.precio < 600
let resultado2 = carrito.filter( producto => producto.nombre === 'Celular' ); // Traerte el celular
let resultado3 = carrito.filter(producto => producto.nombre !== 'Laptop'); // Todos menos la laptop
console.log(resultado);
console.log(resultado2);
console.log(resultado3);
////////////////////////////////////////////////////////////////////////////////////////////////

// con un foreach seria algo asi... dicimulamos un FInd
let resultado = '';
carrito.forEach((producto, index) => {
if(producto.nombre === 'Bocinas') {
resultado = carrito[index]
}
});
console.log(resultado);

// con .find seria
find llama una sola vez cuando se cumple la condicion y si hay mas de 2 solo trae el primero
const resultado2 = carrito.find( producto => producto.nombre === 'Bocinas');
console.log(resultado2);
//////////////////////////////////////////////////////////////////////////////////////////////////////

#### En este video estaremos viendo every...

*  Every es raro, ya que todos los elementos del arreglo deberán cumplir esa condición..

```javascript
const carrito = [
    { nombre: 'Monitor 20 Pulgadas', precio: 500},
    { nombre: 'Televisión 50 Pulgadas', precio: 700},
    { nombre: 'Tablet', precio: 300},
    { nombre: 'Audifonos', precio: 200},
    { nombre: 'Teclado', precio: 50},
    { nombre: 'Celular', precio: 500},
    { nombre: 'Bocinas', precio: 300},
    { nombre: 'Laptop', precio: 800},
];
```

* con un foreach seria algo asi...
```javascript
let cumple = true;
carrito.forEach( producto => {
    if(producto.precio > 700) {
        cumple = false;
        return
    }
    })

console.log(cumple);

const resultado = carrito.every(producto => producto.precio < 1000); // Mil se cumple, 700 no...
console.log(resultado);

```
//////////////////////////////////////////////////////////////////////////////////////////////////

####  En este video veremos como unir 2 arreglos, para ello existe un arreay method llamado .concat

```javascript
const meses = ['Enero', 'Febrero', 'Marzo', 'Abril', 'Mayo', 'Junio'];
const meses2 = ['Julio', 'Agosto', 'Septiembre', 'Octubre', 'Noviembre', 'Diciembre'];
```

* Unir 2 arreglos con concat...
```javascript
const meses3 = meses.concat(meses2);
console.log(meses3);
```

* Existe otra forma... que es con rest operator o spread operator..
```javascript
const meses4 = [...meses,...meses2 ,'otromes']; // Tienes que asegurarte de que sean arrays cuando usas ... 'Otro mes'
console.log(meses4)
```

# REST OPERATOR (...)
*  Un poco más sobre el rest operator...

*  El rest operator es muy útil para crear un nuevo arreglo sin modificar el original...
```javascript
const meses = ['Enero', 'Febrero', 'Marzo', 'Abril', 'Mayo', 'Junio'];

const carrito = [
    { producto: 'Monitor 20 Pulgadas', precio: 500},
    { producto: 'Televisión 50 Pulgadas', precio: 700},
    { producto: 'Tablet', precio: 300},
    { producto: 'Audifonos', precio: 200},
    { producto: 'Teclado', precio: 50},
    { producto: 'Celular', precio: 500},
    { producto: 'Bocinas', precio: 300},
    { producto: 'Laptop', precio: 800},
];
```

*  Si tienes 2 arreglos los unes como vimos en el video anterior, pero digamos que tienes un arreglo y quieres añadir un elemento al final que es un string utilizarias.

```javascript
const meses2 = [...meses, 'Julio'];
console.log(meses);
console.log(meses2); // Recuerda esto no modifica el arreglo original como si haria push y eso es muy útil en un tipo de programación llamada funcional.
```


* O al inicio... en lugar de utilizar unshift,
```javascript
const meses3 = ['Julio',...meses ];
```


*  O tal vez quieres añadir un objeto a un arreglo de objetos al final
```javascript
const producto = {producto: 'Disco Duro', precio: 300};
const carrito2 = [...carrito, producto];
console.log(carrito2);
```

*  o al inicio
```javascript
const carrito3 = [producto, ...carrito];
console.log(carrito3);
```


# DOM
* 01- Vamos a abrir el capitulo 13-DOM y abrirlo en Live server

* Lo primero que haremos sera crear una carpeta llamada js / y en ella colocar el archivo scripts.js

```javascript
let elemento;

elemento = document; // selecciona todo documento del html
elemento = document.all; // seleciona todas las etiquetas que estamos utulizando en el html div h1 <a> todas
elemento = document.all[0]; //
elemento = document.head; // todo lo que sea Head y sus hojas de estilo
elemento = document.body; // todo lo que sea dentro de la etiqueta boddy
elemento = document.domain; // dominio q localhost estas
elemento = document.URL; //
elemento = document.characterSet;
elemento = document.contentType;
elemento = document.forms;// formularios como los de buscar es como un arreglo de acceso
elemento = document.forms[0];// entramos a la selecion
elemento = document.forms[0].id; // selecionamos el id del formulario
elemento = document.forms[0].method;// selecionamos los metodos POST GET
elemento = document.forms[0].action; // selecionamos a la accion

elemento = document.links; // selecciona todos los enlaces o registrados html coleccion
elemento = document.links[4].id;// seleccionamos el el HTML
elemento = document.links[4].classList;// clases de ese html como fuese un INDICE
elemento = document.links[4].className;// te selecciona como fuese un string

elemento = document.forms[4].classList; // accedemos a las clases que tiene ese formulario
elemento = document.forms[4].classList[0];

elemento = document.images; // seleciona las imagenes todas

elemento = document.scripts; // selecciona todas las scripst
elemento = document.scripts[2].getAttribute('src');

console.log(elemento);
```

////////////////////////////////////////////////////////////////////////////////////////////////////////////////

// Seleccionando el header...getElementsByClassName **\*\***\*\***\*\*** SOLO CLASES

                // Todos tus selectores inician con document...
                // Es muy importante las mayusculas y minusculas...

const header = document.getElementsByClassName('header'); // nos permite selecionar los que tenga un nombre y una clase y escribirlo como lo tenemos en el html
console.log(header);

const hero = document.getElementsByClassName('contenido-hero');
console.log(hero);

// Como las classes se pueden repetir, obviamente todas las coincidencias de classes se asignaran a contenedores.
const contenedores = document.getElementsByClassName('contenedor');
console.log(contenedores);

// Si una clase no existe, no va a retornar nada... como una array vacia
const noExiste = document.getElementsByClassName('no-existe');
console.log(noExiste);

///////////////////////////////////////////////////////////////////

# getElementById *********************************solo ID

* En este video estaremos viendo como seleccionar un elemento por su ID, recuerda los ID's solo se deben utilizar uno con ese mismo nombre por documento...

```javascript
const formulario = document.getElementById('formulario') //;Añadir un ID 2 veces, seleccionara el primero que encuentre... si hay 2 id iguales
console.log(formulario);

const noExiste = document.getElementById('no-existe'); // Si no exist eestará vacio
console.log(noExiste);
```


//////////////////////////////////////////////////////////////////

querySelector class y id retorna 1 y se usa como buscado de css

// querySelector va a retornar máximo 1 elemento, si hay múltiples coincidencias solo va a retornar el primero...

const card = document.querySelector('.card'); // QuerySelctor utiliza una sintaxis como de selector de CSS, por lo tanto si deseas seleccionar una clase, debe tener un punto al inicio...

// nota como a pesar de tener múltiples cards, solo selecciona 1

console.log(card);

// al ser una sintaaxis tipo CSS puedes utilizar selectores más especificos...

const info = document.querySelector('.premium .info');
console.log(info);

// Seleccionar el segundo card... de hospedaje
const segundoCard = document.querySelector('.hospedaje .card:nth-child(2)');
console.log(segundoCard);

// Ahora estas son classes, veamos como seleccionar un ID
const formulario = document.querySelector('#formulario'); // En CSS seleccionas los ID con un signo de numeral..
console.log(formulario);
// También los ID pueden tener selectores especificos como el de arriba, pero recuerda un ID es único asi que no tendría mucho sentido no?

// En CSS seleccionas los ID con un signo de numeral..
const formulario = document.querySelector('.contenido-hero #formulario');
console.log(formulario);

// Si un selector no existe,
const noExiste = document.querySelector('#no-existe');
console.log(noExiste);

// Recuerda que también en CSS puedes seleccionar etiquetas asi que si quieres seleccionar la navegación podrías tener algo asi:
const nav = document.querySelector('nav');
console.log(nav);

//////////////////////////////////////////////////////////////////
querySelectorAll **********************\*\*\*\***********************\*\*\*\***********************\*\*\*\***********************

// la buena noticia es que la sintaxis para selectores es la misma, es decir similar a CSS, con el punto para las classes y el numeral o signo de gato para los ID's, también puedes añadir un selector especifico..

// Pero la diferencia principal, es que querySelectorAll va a retornar todos los elementos que concuerden con el selector y no va a limitarte al primero como querySelector.

// En nuestro HTML hay muchos cards, cuando utilizamos querySelector vimos que retornaba unicamente el primero..

const cards = document.querySelectorAll('.card');
console.log(cards);

// si recuerdas tenemos dos elementos con el id de formulario

const formularios = document.querySelectorAll('#formulario');
console.log(formularios); // Puedes ver quue eso si funciona, sin embargo recuerda que no rescomendable tener el mismo ID más de una vez por docuemnto...

// Si no hay elementos no va a retornar nada

// Si un selector no existe,
const noExiste = document.querySelectorAll('#no-existe');
console.log(noExiste);

////////////////////////////////////////////////////////////////
IMPRIMIENDO Y CAMBIANDO TEXTO Y IMAGENES **********\*\*\*\***********\***********\*\*\*\***********

const encabezado = document.querySelector('.contenido-hero h1');
// console.log(encabezado);

// Si deseas acceder al texto hay 3 formas de hacerlo...
console.log(encabezado.innerText); // si le ponemos a ese elemento visibility: hidden; en el CSS,
console.log(encabezado.textContent); // entra al texto y modifica
console.log(encabezado.innerHTML); // se trae el html

// Ahora, aquí puedes ver que estoy asignando el Texto a una variable, pero también puedes modificarlo de diferentes formas...

document.querySelector('.contenido-hero h1').textContent = 'Nuevo Heading'

// otra opción seria con una variable.

const nuevoTexto = 'Nuevo Heading'; ///crea la constante y luego la lleva abajo
document.querySelector('.contenido-hero h1').textContent = nuevoTexto;

// También puedes cambiar una imagen...

// No lo hemos visto, pero veamos por ejemplo como acceder a esa imagen...

const imagen = document.querySelector('.card img');
console.log(imagen.src);
// Cambiar la imagen...
imagen.src = 'img/hacer2.jpg';

//////////////////////////////////////////////////////////////////////////////////////////////////////

# CAMBIAR COLOR  AÑADIR CLASES Y ELIMINAR 
* En JavaScript también es posible cambiar el CSS de un elemento, o agregar o quitar classes...

* Vamos a cambiar el color de texto del h1

```javascript
const heading = document.querySelector('h1');
```
// y hay todo un objeto con propiedades CSS que puedes utilizar, si quieres conocerlas todas coloca...

```javascript
console.log(heading.style);
```
```javascript
heading.style.backgroundColor = 'red'; // Nota como las propiedades que le puedes pasar, son similares a las de CSS, con la diferencia de que el guion se elimina y la segunda palabra su primer letra es mayuscula.

heading.style.textTransform = 'uppercase';
heading.style.fontFamily = 'Arial';

// Ahora yo no recomiendo que pongas style, ya que tu archivo JS será muy grande, otra desventaja es que la apariencia debe ser algo que sea responsabilidad del CSS, pero lo que si puedes hacer es agregar o quitar classes..

// Vamos a seleccionar el primer card, puedes ver que tiene un parrafo con una categoria llamada concierto, eso le cambia el color:
const card = document.querySelector('.card');
console.log(card);
console.log(card.classList); // Classlist nos permitirá listar las classes
card.classList.add('nueva-clase'); // te permitirá añadir una clase.. // si deseas añadir múltiples classes debes agregar una coma en cada una

// ahora si deseas eliminar una clase utilizas.remove
card.classList.remove('card'); // de la misma forma si deseas remover múltiples classes tendrías que hacerlo agregando una coma
```

// -----------------------------------Traversing the DOM---------------------------------------------

// Todo en JavaScript esta conectado en el document, la forma en que te moverás entre diferentes elementos se le conoce como Traversing the DOM, ir recorriendolo..

const navegacion = document.querySelector('.navegacion');
console.log(navegacion);

// Cada elemento en la navegación los diferentes elementos se les conoce como Nodos... y podrás listarlos de la siguiente forma...

console.log(navegacion.childNodes); // La diferencia es que childNodes te va a mostrar hasta los espacios en blanco, del html

// también existe algo llamado Children

console.log(navegacion.children) //children te muestra solo los elementos... del html

// Hay mucha información aqui...
console.log(navegacion.children[0].nodeType) // Tipo de Node = 1 es un eleemnto
console.log(navegacion.children[0].nodeName) // Que etiqueta es...

// Por ejemplo si selecciono el primer card...

const card = document.querySelector('.card');
console.log(card.nodeType);
console.log(card.nodeName);

// 1 = Elemento
// 2 - Atributo
// 3 - Text node
// 8 - Commentario
// 9 - Documento
// 10 doctype

// en javascript puedes seleccionar un elemento y navegar en sus diferentes elementos... por ejemplo el card...

console.log(card.children);
console.log(card.children[1]);// Si quieres acceder a ese div con la clase de info puedes colocar...

console.log(card.children[1].children[1]);// Si quieres accedera los elementos hijos de ese info... recuerda puedes anidar las propiedades.

console.log(card.children[1].children[1].textContent);// Acceder al titulo

card.children[1].children[1].textContent = 'Cambiando el Texto con traversing...'// Modificar ese titulo con un traversing

// Intenta cambiar el texto que dice concierto por algo más siguiendo esta sintaxis de ir navegando por el DOM...

// No lo hemos visto, pero veamos por ejemplo como acceder a esa imagen...
console.log(card.children);
console.log(card.children[0]);
console.log(card.children[0].src);

// Cambiar la imagen...
card.children[0].src = 'img/hacer2.jpg';

// Children es una buena forma de acceder a los elementos por su posición, pero supongamos que de nuestra navegación queremos acceder al primer o último enlace...

console.log(navegacion.lastChild);
console.log(navegacion.lastElementChild);

console.log(navegacion.firstChild)// Si desesa acceder al primero

console.log(navegacion.firstElementChild);// su deceas acceder al ultimo

navegacion.firstElementChild.textContent = 'Nuevo Enlace...'// Cambiar el primer texto...

-

// En el video anterior vimos como hacer traversing de un elemento padre hacia el hijo, JavaScript también te permite seleccionar un elemento hijo e ir navegando hacia el padre...

// vamos a seleccionar el primer enlace...
const enlace = document.querySelector('a');
console.log(enlace);

// Hay diferente sformas...

console.log(enlace.parentNode)
console.log(enlace.parentElement)

// En algunos casos ambos van a dar el mismo resultado, en otros recuerda el espacio es importante...

console.log(enlace.parentElement.parentElement)// También puedes ir al padre del padre... y de hijo a padre

// En JavaScript también es posible de hacer traversing a elementos que estan en el mismo nivel , digamos el vecino aunque en javascript se les conoce como hermanos...

console.log(enlace);
console.log(enlace.nextElementSibling); // siguiente si esta en el mismo nivel esto se llama TRAVERSING
console.log(enlace.nextElementSibling.nextElementSibling); // pasara 2 veces el siguiente

console.log(card.nextElementSibling);

const ultimoCard = document.querySelector('.card:nth-child(4)');
console.log(ultimoCard)

console.log(ultimoCard.previousElementSibling);// También hay una forma de ir digamos en la otra dirección... VAMOS A la posicion 4 y esto nos dirigira al 3

///////////////////////////////////////////////////////////////////////////////////////
// Después de una super extensa explicación de Traversing y acceder a elementos, veamos como eliminar elementos del DOM
// Es muy común no? cuando borras una foto de facebook o un tweet se elimina automaticamente, también cuando quitas elementos del carrito de compras de amazon.
// Cuando le diste me gusta a una foto por accidente y le quitas el like, también hay un cambio, así que sin duda eliminar elementos llega a ser muy común..
// Hay 2 formas de eliminar, una es eliminar un elemento por si mismo y la otra es eliminarlo desde el padre...

const primerEnlace = document.querySelector('a');
primerEnlace.remove();

// La otra forma es por el padre..
const navegacion = document.querySelector('.navegacion');
// console.log(navegacion.children);
// navegacion.removeChild(navegacion.children[2]);// el sigueinte paso es identificar el elemento a borrar..

// Otra forma es creando una variable...
const borrar = navegacion.children[2]
navegacion.removeChild(borrar);

// Como resumen recuerda hay 2 formas de eliminar elementos, uno es por el elemento por si mismo y el otro requiere el padre y la referencia del hijo..

//////////////////////////////////////////////////////////////////////////////////////
AGREGANDO DIV IMAGENES AL DOM ****************\*\*****************\*\*\*****************\*\*****************

// Finalmente otro tema importante cuando trabajas con el DOM, es la creación de HTML desde JavaScript..

// Cuando publicas un tweet, tienes un textarea que al enviarlo se agrega al listado de tweets, de ahi la gente comienza a darle me gusta, así que veamos como hacerlo generar HTML desde JavaScript...

// Y no te preocupes si todo lo que vemos en este video no queda claro, estaremos practicando mucho lo que es el DOM Scripting ya con muchos otros proyectos...

// Vamos a crear un nuevo enlace... lo primero que hay que hacer es crear el elemento HTML, en este caso un enlace...

const enlace = document.createElement('A'); // si vamos a crear una etiqueta o generando archivos cosas d HTML

// Segundo paso es crear el texto del enlace no? lo haremos con textContent

enlace.textContent = 'Nuevo Enlace'; // agrega un texto a la etiqueta

// Despues vamos a asignar una ruta
enlace.href = '/nuevo-enlace'; // añadiendo HREF
// Finalmente se agrega el enlace donde deseas mostrarlo...
enlace.target = '\_blank' //\_blank : Carga la URL en un nuevo contexto de navegación
// Si quieres agregar una clase
enlace.classList.add('enlace'); // agregando nueva clase

enlace.setAttribute('data-enlace', 'nuevo-enlace') // atributos de html

enlace.onclick = miFuncion; // crear una funcion al dar click

const navegacion = document.querySelector('.navegacion');
// console.log(navegacion.children); // vemos la posiciones
//navegacion.appendChild(enlace); // APPENDCHILD es como crear nuevo hijo a NAVEGACION del menu por ejemplo y su nuevo hijo sera enlace
navegacion.insertBefore(enlace, navegacion.children[1]); // colocar dentro del NAVEGACION la posicion que quiero poner mi nuevo ENLACEs

/_function miFuntion(){
alert('diste click') // hago mi funcion y llamo cuando den click
}_/

console.log(enlace);

// Vamos a crear un segundo ejemplo, crearemos uno de nuestros cards... sin duda será algo más complejo...

// crear los 3 parrafos.

const parrafo1 = document.createElement('P'); // crea los parrafos
parrafo1.textContent = 'Concierto'; // inserta texto
parrafo1.classList.add('categoria'); // fon-size tamaño
parrafo1.classList.add('concierto'); // color

// Segundo parrafo
const parrafo2 = document.createElement('P');
parrafo2.textContent = 'Concierto de Rock';
parrafo2.classList.add('titulo'); // titulo clase dada por css y html letras grandes

// 3er parrafo...
const parrafo3 = document.createElement('p');
parrafo3.textContent = '$800 por pesrona'; // precio
parrafo3.classList.add('precio'); // sub titulo de css

// crear el div...
const info = document.createElement('div'); // tiene la clase info llamaos a info y creamos un div
info.classList.add('info'); // agrega el div a INFO

info.appendChild(parrafo1) // agrega los parrafos anteriores
info.appendChild(parrafo2)
info.appendChild(parrafo3);

// Vamos a crear la imagen
const imagen = document.createElement('img');
imagen.src = 'img/hacer2.jpg';
//imagen.alt = " texto alternativo";
// Crear el Card..
const card = document.createElement('div');
card.classList.add('card');

// Vamos a asignar la imagen al card...
card.appendChild(imagen); // agregamos imagen al card

// y el info
card.appendChild(info);// agregamos info al card

// Insertarlo en el HTML...
const contenedor = document.querySelector('.hacer .contenedor-cards');
contenedor.appendChild(card); // al inicio info
// contenedor.insertBeforse(card , contenedor.children[0] ) // elegimos la posicion que queremos poner

console.log(parrafo1);
console.log(parrafo2);

///////////////////////////////////////////////////////////////////////////////////////////////////
MOSTRAR Y OCULAR BOTON CON CLASES CSS ACTIVO A DESATIVO ******\*\*******\*******\*\*******DOM
// No siempre estarás haciendo traversing a tu dom,

const btnFlotante = document.querySelector('.btn-flotante'); // llamamos al boton

const footer = document.querySelector('.footer'); // llamamos es lo que sale para arriva

btnFlotante.addEventListener('click', mostrarOcultarFooter); // cuando de click hacer funcion o evento

function mostrarOcultarFooter() {
if( footer.classList.contains('activo') ) { // Constaind busca si es que esta activo SINO ELSE AGREGA el ACTIVO y cuando vuelva a recorrer ya esta activo aqui y muestra recien el cuadro
footer.classList.remove('activo'); // // remueve el activo
this.classList.remove('activo'); // // remueve activo del boton y color
this.textContent = 'Idioma y Moneda'; // cuando no esta activo
} else {
footer.classList.add('activo'); // agrega ACTIVO
this.classList.add('activo'); // agrega la clase de activo y el color
this.textContent = 'X Cerrar'; // cuando esta activo
}
}
}
//////////////////////////////////////////////////////////////////////////////////////////////////

AQUI muestra el 1,3,2 el DOMContentLoaded espera q todo cargue
console.log(1)
document.addEventListener('DOMContentLoaded', () => {
console.log(2);
}) // Nota todos los eventos que hay disponibles
console.log(3);

/////////////////////////////////////////////////////////////////////////////////////////////////
MAUS **\*\*\*\***\*\***\*\*\*\***

// En este video estaremos viendo eventos que ocurren con el mouse

const nav = document.querySelector('.navegacion');

// vamos a registrar el eventListener para el nav..

nav.addEventListener('mouseenter', () => {
console.log('entrando a navegacion')

    nav.style.backgroundColor = 'white'; // color

});

nav.addEventListener('mouseout', () => {
console.log('saliendo de la navegacion');

    nav.style.backgroundColor = 'transparent';

})

// otros eventos abarcan...

// mousedown - // cuando presionamos
// click - similar, de hecho es probablemente el más utilizado..
// dbclick - doble click como cuando quieres abrir un archivo
// mouseup - al soltar
// mauseenter - cuando pasas sobre el
// mauseout -cuando sales sobre el



# TECLADO

En este video estaremos viendo eventos que suceden con el teclado, es decir cuando el usuario escribe en un input...

tenemos un formulario

```javascript
const busqueda = document.querySelector('.busqueda');

// busqueda.addEventListener('input', () => {
// console.log('escribiendo...');
// })

// keydown - cuando presionas una tecla
// keyup - Cuando sueltas la tecla...
// blur - cuando sales del input - ideal para validación...
// También hay eventos para cortar copiar y pegar

// cut cuando cortan
// copy
// paste cuando pegas algo
// input - cuando se ejecutan todas las que aquí se muestran... incluyendo cortar, pegar y copiar menos el blur
// e = a o leer evento

// Ahora, no tiene mucha utilidad enviar a la consola un mensaje no? lo ideal seria saber el texto que se escribe o poderlo leer...

// busqueda.addEventListener('input', e => { // (e)evento
// console.log(e); // Mucha información...
// console.log( e.type ); // Te dira sobre que elemento estamos trabajando...
// console.log(e.target); // el input completo...todos las etiquetas

// console.log(e.target.value) // lo que el usuario escribe...

// })

// También puede ser como función...

busqueda.addEventListener('input', leerInput);

function leerInput(e) {
console.log(e); // Mucha información...
console.log( e.type ); // Te dira sobre que elemento estamos trabajando...
console.log(e.target); // el input completo...
console.log(e.target.value) // lo que el usuario escribe...

}
```



# SUBMIT

Veamos los eventos para un formulario, básicamente es uno pero es muy importante y merecia su propio video...

Cuando envias un formulario usualmente lo que este en el action, es la página que se abre...

```javascript

const formulario = document.querySelector('.formulario');


formulario.addEventListener('submit', e => {
    // SUBMIT es como cuando alguien preciona el boton o input que tiene el SUBMIT

    e.preventDefault(); // PreventDefault es evitar que el navegador realice la acción por default, en este caso ir al action...

    //  e.preventDefault();  previene la accion que tenia q hacer y le damos una nueva accion nosotros o lo q requerimos

    // Usualmente utilizaras preventDefault para validar el formulario antes de enviarlo a un servidor

    // Crear consultas Ajax entre otras cosas o api antes de ir al enlace predestinado

    console.log('enviando...');


    // Mucha información valiosa en este e...
    console.log(e);

    console.log(e.target.method)
    console.log(e.target.action)

}

const formulario = document.querySelector('#formulario');


formulario.addEventListener('submit', validarFormulario){

    function validarFormulario(e){ // siempre va (e) ya que arriva lo llama
        e.preventDefault();

        console.log('enviando...');
        console.log(e);

        console.log(e.target.method)
        console.log(e.target.action)
    }


}
```

# SCROLL

- En este video estaremos viendo eventos que suceden con el scroll del sitio web...

- Es muy común que muchos sitios agreguen funcionalidad de que al dar scroll y llegar a ver un elemento este tenga alguna animación, eso se hace con eventos en el mouse..

```javascript
window.addEventListener("scroll", () => {
  // console.log('scrolling...');

  // Detectar el Scrolling vertical...

  // const pxScroll = window.scrollY;
  // console.log(pxScroll);

  // window.scrollY = cuantos pixeles hay de arriba y ir bajando

  // Detectar un elemento al dar scroll...

  const premium = document.querySelector(".premium");

  const ubicacion = premium.getBoundingClientRect(); // Este método te da el tamaño de un elemento y su ubicación respecto a la ubicación actual..en movimiento de html de arriba para abajo
  // console.log(ubicacion);

  if (ubicacion.top < 100) {
    console.log("Ya esta visible"); // cuando bajemos la pagina estara visibile y podremos ser espesifico si pondremos un css o imagen en ese scroll
  } else {
    console.log("Aún no esta visible.. da mas scroll");
  }
});
```

# STOP DE CLICK EVENT BUBLING

prevenir 1 click dado en 3 enlaces y q sea uno en cada uno

- Veamos lo que se conoce como Event Bubbling...

Event Bubling es cuando presionas en un evento, pero ese evento se propaga por muchos otros dando resultados inesperados

Tenemos diferentes cards, con información...
vamos a crear 3 selectores

```javascript
const cardDiv = document.querySelector(".card");
const infoDiv = document.querySelector(".info");
const titulo = document.querySelector(".titulo");

cardDiv.addEventListener("click", (e) => {
  e.stopPropagation();
  console.log("click card");
});
infoDiv.addEventListener("click", (e) => {
  e.stopPropagation();
  console.log("click info");
});

titulo.addEventListener("click", (e) => {
  e.stopPropagation();
  console.log("click titulo");
});
```

# DELEGATION

Nos dirigimos a la direcion q damos click
Otra opción que a mi me gusta mucho es aplicar algo llamado delegation..

```javascript
const cardDiv = document.querySelector('.card');

cardDiv.addEventListener('click', e => {  evento click
    if(e.target.classList.contains('titulo')) { // si se da click en TITULO mostrar "click titulo// e.targe muestra las etiquetas .clasllist las clases . constains mostrara el css q hay en ese html
        console.log('click titulo');
    }
    if(e.target.classList.contains('info')) { // si diste click en info mostrar "click info"
        console.log('click info');
    }
});
```

# OTRA FORMA PARA EVITAR LA PROPAGACION

- Evitar la propagación con contenido creado...

```javascript
const parrafo1 = document.createElement("P");
parrafo1.textContent = "Concierto";
parrafo1.classList.add("categoria");
parrafo1.classList.add("concierto");
```

- Segundo parrafo

```javascript
const parrafo2 = document.createElement("P");
parrafo2.textContent = "Concierto de Rock";
parrafo2.classList.add("titulo");
```

- Tercer parrafo...

```javascript
const parrafo3 = document.createElement("p");
parrafo3.textContent = "$800 por persona";
parrafo3.classList.add("precio");

parrafo3.onclick = nuevaFuncion(1); // nuevo click para dar una funcion
```

- crear el div

```javascript
const info = document.createElement("div");
info.classList.add("info");
info.appendChild(parrafo1);
info.appendChild(parrafo2);
info.appendChild(parrafo3);
```

- Vamos a crear la imagen

```javascript
const imagen = document.createElement("img");
imagen.src = "img/hacer2.jpg";
```

- Crear el Card..

```javascript
const contenedorCard = document.createElement("div");
contenedorCard.classList.add("contenedorCard");
```

- Vamos a asignar la imagen al card...

```javascript
contenedorCard.appendChild(imagen);
```

- y el info

```javascript
contenedorCard.appendChild(info);
```

- Insertarlo en el HTML...

```javascript
const contenedor = document.querySelector(".hacer .contenedor-cards");
contenedor.appendChild(contenedorCard); // al inicio info
```

```javascript
function nuevaFuncion(id) {
  // CUANDO A SIDO DADO UN CLICK mostrar id
  console.log("click..", id);
}
```

# LOCALSTORAGE AGREGAR

- añadir algo a sessionstorage

```javascript
sessionStorage.setItem("nombre", "Pablo");
```

- Local Storage solo soporta strings, no soporta arrays ni objetos pero puedes almacenarlos convirtiendolos a string..

```javascript
const producto = {
  nombre: 'Monitor 24"',
  precio: 300,
};
```

- combertimos un objeto en string agregando al localstorage

```javascript
const productoString = JSON.stringify(producto);
localStorage.setItem("productoJSON", productoString);
```

- Lo mismo con un array a string

```javascript
const meses = ["Enero", "Febrero", "Marzo"];
localStorage.setItem("meses", JSON.stringify(meses));
```

# LOCALSTORAGE OBTENER DATOS

### Aca vamos aprender como obtener los datos de Local storage

- Esto es para obtener el valor

```javascript
const nombre = localStorage.getItem("nombre");
console.log(nombre);
```

- Obetener el STRING y pasarlo a OBJETO

```javascript
const productoJSON = localStorage.getItem("productoJSON");
console.log(JSON.parse(productoJSON));
```

- De STRING a ARREGLO

```javascript
const meses = JSON.parse(localStorage.getItem("meses"));
console.log(meses);
```

# LOCALSTORAGE

### REMOVER ACTUALIZAR Y ELIMINAR

- Aca vamos a ver como eliminar elementos del local storage...

```javascript
localStorage.removeItem("nombre");
```

- En cuanto a toda laf uncionalidad d eun CRUD, nos haria falta un update, no hay como tal un Update... lo que podrías hacer es...

```javascript
const mesesArray = JSON.parse(localStorage.getItem("meses"));
console.log(mesesArray);
```

- agregar

```javascript
mesesArray.push("nuevo Mes");
console.log(mesesArray);
```

- actualiza el localstorage

```javascript
localStorage.setItem("meses", JSON.stringify(mesesArray));
```

- eliminar

```javascript
localStorage.clear();
```

# PROTOTYPE

### **Clases**:

Modelo a seguir

### **Objeto**:

Es una instancia de una clase cuando ya tiene nombre ese objeto.

### **atributos**:

Es una caracteristica o propiedad del objeto (son variables dentro de un objeto)

### **Metodos**:

Son las acciones que un objeto puede realizar objeto unico que hereda atributos para otras metodos.

### **Prototype**:

Son como datos dentro de objetos para ser usado por metodos con funciones. Por que con arrow no puede, solo se usa local mente no globalmente.

- Tambien se puede usar la herencia de datos para otros prototypes

### **Clases**:

Es casi igual que prototype solo que se diferencia en herencia para heredar usan la palabra "extends classObjeto anterior"

### **Privado y Publico**:

A la variable se lepone un # para que sea privado por ejemplo : #nombre solo se puede acceder por la clase

### **CREANDO UN SET** (EJEMPLO)

```javascript
const mySet = new Set();

mySet.add(1);
mySet.add(5);
mySet.add("some text");

const o = { a: 1, b: 2 };
mySet.add(o);

mySet.add({ a: 1, b: 2 }); // La variable "o" referencia a otro objeto, por lo que agrega otro valor.

mySet.has(1); // true
mySet.has(3); // false, 3 no ha sido añadido al Set
mySet.has(5); // true
mySet.has(Math.sqrt(25)); // true
mySet.has("Some Text".toLowerCase()); // true
mySet.has(o); // true

mySet.size; // 5

mySet.delete(5); // Elimina 5 del Set
mySet.has(5); // false, 5 fue eliminado

mySet.size; // 4, sólo removimos un valor
console.log(mySet); // Set {1, "some text", Object {a: 1, b: 2}, Object {a: 1, b: 2}}
```

- Un set te permite crear una lista de valores sin duplicados.

Pocas veces los veo que se utilizan, muchas personas prefieren crear arreglos y evitar duplicados, pero sería más sencillo con un set... de hecho en algunas ocasiones termina siendo mejor opción que un arreglo o un objeto

```javascript
let carrito = new Set();

carrito.add("Camisa");
carrito.add("Disco #1");
carrito.add("Disco #2");
carrito.add("Disco #3");
carrito.add("Disco #3");

console.log(carrito.size);
```

- En un arreglo

```javascript
let numeros = new Set([1, 2, 3, 4, 5, 6, 7, 3, 3, 3, 3]);
console.log(numeros.size);
```

```javascript
let carrito = new Set();
carrito.add("Camisa");
carrito.add("Disco #1");
carrito.add("Disco #2");
carrito.add("Disco #3");
carrito.add("Disco #3");
```

- Comprobando que un valor existe en el set.

```javascript
console.log(carrito.has("Camisa"));
```

- Eliminando del set

```javascript
console.log(carrito.delete("Camisa"));
console.log(carrito.has("Camisa"));
console.log(carrito);
```

- Limpiar un set

```javascript
carrito.clear();
console.log(carrito);
```

- Foreach a un set

```javascript
carrito.forEach((producto) => {
  console.log(producto);
});
```

- Foreach a un set

```javascript
carrito.forEach((producto, index, pertenece) => {
  console.log(`${index} : ${producto}`);
  console.log(pertenece === carrito); // nombre de la variable
});
```

- Convertir un set a un arreglo...

```javascript
const arregloCarrito = [...carrito];
console.log(arregloCarrito);
```
