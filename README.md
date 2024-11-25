* 
{ margin: 0;
  padding: 0;
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;}

body {
  background:linear-gradient(#2F6D72,#2F5472);

  height: 100vh;
  font-family: 'Open Sans', Arial, 'Helvetica Neue', Sans-serif, Verdana, Tahoma;
  font-size: 62.5%;}

ul {list-style-type: none;}

a {
  color: #1396e1; 
  text-decoration: none;
}

.clearfix:after {
  content: '';
  display: block;
  width: 0;
  height: 0;
  clear: both;
}
 .main-wrapper {
  display: block;
  margin: 50px auto 40px;
  width: 960px;
 }

 .main-wrapper input[type="radio"] {
  display: none;
 }

 
 .main-title {
  color: #242424;
  font: 400 3.2em 'Open Sans', Arial, Sans-serif, Verdana;
  text-align: center;
 }

 .main-title a {
  color: #1396e1;
  font-size: 0.5em;
  font-weight: 700;
 }

 /* Lista de Categorias 
 --------------------------------------------*/
 .list-category {
  display: block;
  text-align: center;
  margin-top: 20px;
 }

.list-category li {
  display: inline-block;
  font-size: 1.6em;
}

.list-category label {
  display: inline-block;
  color: #E5E5E5;
  cursor: pointer;
  background: #3e4257;
  -webkit-box-shadow: inset 0 -2px 0 rgba(0,0,0,0.25);
  box-shadow: inset 0 -2px 0 rgba(0,0,0,0.25);
  -webkit-border-radius: 3px;
  -moz-border-radius: 3px;
  border-radius: 3px;
  padding: 12px 16px;
  -webkit-transition: all 0.2s ease;
  -o-transition: all 0.2s ease;
  transition: all 0.2s ease;
}

/* Imagenes / En este caso divs de colores :C
 --------------------------------------------------*/
 .list-images {
  color: #000;
  display: block;
  margin-top: 40px;
  text-align: center;
 }

 .list-images li {
  opacity: 0.3;
  width: 200px;
  height: 120px;
  margin: 5px;
  display: inline-block;
  border: 4px solid #FFF;
  -webkit-box-shadow: 0 0 0 1px rgba(0,0,0,0.15);
  box-shadow: 0 0 0 1px rgba(0,0,0,0.15);
  color: #FFF;
  font-size: 1.5em;
  font-weight: 700;
  -webkit-transform: scale(0.9);
  -ms-transform: scale(0.9);
  -o-transform: scale(0.9);
  transform: scale(0.9);
  -webkit-transition: all 0.4s ease;
  -o-transition: all 0.4s ease;
  transition: all 0.4s ease;
 }

.list-images li span {
  position: relative;
  top: 40px;
}

.list-images .type-webdesign {background: #3fab91;}
.list-images .type-webdevelopment {background: #ffbb45;}
.list-images .type-graphicdesign {background: #db559a;}
.list-images .type-javascript {background: #994356;}

/* Estilos cuando un radio esta seleccionado
 --------------------------------------------------*/
#all:checked ~ .list-category label[for="all"],
#webdesign:checked ~ .list-category label[for="webdesign"], 
#webdevelopment:checked ~ .list-category label[for="webdevelopment"], 
#graphicdesign:checked ~ .list-category label[for="graphicdesign"], 
#javascript:checked ~ .list-category label[for="javascript"] {
  background: #1396e1;
  color: #FFF;
}

/* Filtramos las clases mediante el selector ~
 --------------------------------------------------*/
#all:checked ~ .list-images li {
  opacity: 1;
  -webkit-transform: scale(1);
  -ms-transform: scale(1);
  -o-transform: scale(1);
  transform: scale(1);
}

#webdesign:checked ~ .list-images .type-webdesign,
#webdevelopment:checked ~ .list-images .type-webdevelopment,
#graphicdesign:checked ~ .list-images .type-graphicdesign,
#javascript:checked ~ .list-images .type-javascript {
  opacity: 1;
  -webkit-transform: scale(1);
  -ms-transform: scale(1);
  -o-transform: scale(1);
  transform: scale(1);
}



