# patio-mundo
Prueba de proyecto de trabajo en grupo 
Se necesita cambiar el cssdel uso de grids por mediao del gridgenerator que se generó en: https://grid.layoutit.com/
ya que este solo ayuda a crear los grids, sin ser responisvos.
El o los estilos recomendados fueron dados a conocer con display:grids
En el sideño web con LESS: Avenue Fashion, donde se aplica grids:
Ejemplo:
//itmes en 3 columnas, pero abajo hay 4 imagenes
.items, .itemssFour{
	display: grid;
	grid-template-columns: auto auto auto;//divide en tres columnas
	//articulos
	article{
		background: @grisSuave2;
		.margen(1em);
		.imgItems{
			float: left;
			.anchoImg(160px, 100%);
			.margen(.8em);
		}
		.fo{
			color: @grisOscuro;
			.negrita(bold);
			.margenInterno(.5em);
		}
	}
	.double{
		//por ocupar mas espacio se uso esta clase y mejorar su apariencia JANES LOOKBOOK
		background:@grisSuave;
		.margenInterno(2em);
	}
}
//reconfigurando itemsFour
.itemsFour{
	grid-template-columns: auto auto auto auto;//divide en 4 columnas	
}
