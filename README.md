# CssAda

#FlexBox
<style>
    section {
        display: flex; /* establecemos la propiedad flex en la sección */
        justify-content: space-between; /* distribuimos uniformemente los elementos a lo largo de la fila */
    }

    div {
    background-color: blue;
    color: white;
    padding: 10px;
    font-size: 20px;
    text-align: center;
    }

</style>
<section>
    <div>Elemento 1</div>
    <div>Elemento 2</div>
    <div>Elemento 3</div>
  </section>

#Grid
<style>
section {
  display: grid; /* establecemos la propiedad grid en la sección */
  grid-template-columns: repeat(4, 300px); /* establecemos tres columnas con una anchura altura fija de 100px */
  grid-template-rows: repeat(3, 100px); /* establecemos tres filas con una altura fija de 100px */
  gap: 10px; /* establecemos un espacio uniforme de 10px entre los elementos */
}

div {
  background-color: blue;
  color: white;
  padding: 10px;
  font-size: 20px;
  text-align: center;
}
</style>

<section>
    <div>Elemento 1</div>
    <div>Elemento 2</div>
    <div>Elemento 3</div>
    <div>Elemento 4</div>
    <div>Elemento 5</div>
    <div>Elemento 6</div>
    <div>Elemento 7</div>
    <div>Elemento 8</div>
    <div>Elemento 9</div>
</section>

#Posicionamiento

<style>
.contenedor {
  position: relative; /* establecemos una posición relativa en el contenedor */
  width: 300px;
  height: 200px;
  background-color: red;
}

.cuadro {
  position: absolute; /* establecemos una posición absoluta en el cuadro */
  top: 10px; /* colocamos el cuadro 10px desde el borde superior del contenedor */
  right: 10px; /* colocamos el cuadro 10px desde el borde derecho del contenedor */
  width: 50px;
  height: 50px;
  background-color: green;
}

p {
  position: static; /* posición por defecto */
  color: blue;
  font-size: 18px;
}

.relativo p {
  position: relative; /* establecemos una posición relativa en el párrafo */
  top: 10px; /* movemos el párrafo 10px hacia abajo */
  left: 70px; /* movemos el párrafo 20px hacia la derecha */
  color: blue;
  font-size: 18px;
}

button {
  position: fixed; /* fijamos el botón en la ventana del navegador */
  bottom: 10px; /* colocamos el botón 10px desde la parte inferior de la ventana */
  right: 10px; /* colocamos el botón 10px desde el borde derecho de la ventana */
  background-color: blue;
  color: white;
  font-size: 18px;
  padding: 10px 20px;
}
</style>
<h1>Absolute</h1>
<div class="contenedor">
    <div class="cuadro"></div>
    <div style="margin-top: 50px">Texto 2</div>
</div>

<hr>

<div>
    <h1>Static</h1>
    <p>Este es un párrafo de texto</p>
</div>

<hr>

<div class="relativo">
    <h1>Relative</h1>
    <p>Este es un párrafo de texto</p>
</div>

<hr>
<div>
    <h1>Fixed</h1>
    <button>Click aquí</button>
</div>


#Grid2
<style>
.container {
  display: grid;
  grid-template-columns: auto auto auto;
  grid-gap: 10px;
  
  padding: 10px;
  border-radius: 10px;
}
.container > div {
  border: 1px solid #fff;
  padding: 40px;
  font-size: 30px;
  text-align: center;
}
.item1, .item6 {
  grid-column-start: 1;
  grid-column-end: 3;
}
</style>

<div class="container">
    <div class="item1">Banner</div>
    <div class="item2"></div>
    <div class="item3">Nombre:</div>
    <div class="item4"><input type="text"></div>
    <div class="item5"></div>
    <div class="item6"></div>
    <div class="item7"><button>GUARDAR</button></div>
</div>


