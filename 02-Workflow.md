


# Workflow Juan Carlos
A continuación se detallan los pasos de flujo de trabajo utilizado para la investigación. En primer lugar ocupamos [Obsidian](http://obsidian.md.com). Veamos:

## 1. Método Zettelkasten

**Fase 1** : Consta de que una vez vas leyendo la bibliografía y tienes tus anotaciones, al final las lees y le asignas un tag al tema que pertenecen. Esto es lo que hacía Niklas Luhman ( Sociologo Aleman) para ordenar sus anotaciones en cajas.
**Fase 2**: Realizar un resumen de las notas que tomastes durante el día y asignas un tema.
**Fase 3**: Crear nuevos Zettels o grandes notas. 

Por ej. Estoy escribiendo una nota con la información extraída de Hyppollito et al. (2015), Willner et al. (2009), Richter et al., (2017). Estas ya son 3 notas separadas, al final leo las tres notas y asigno tags. De esos temas, hago block reference en una nueva nota sobre un tema mayor, por ejemplo en la nota de Contexto Geodinámico. De esta manera Contexto Geodinámico se me transforma en un nuevo Zettel 

## 2. Método: jcmoral.obs

- [ ] **Paso 1** : Descargar paper con Ctrl + Shift + L (Plugin Sci Hub X) luego guardar con el plugin de Zotero. Aunque lo mejor es ingresar el DOI con la varita mágica en Zotero. Se genera la metadata automaticamente.

- [ ] **Paso 1** : Lectura de PDF en Zotero. Trabajar de igual manera todo tipo de docuento pdf en Zotero. Una vez terminado de leer, **trabajar en la metadata** (Se que es dificil, pero es importante para el paso 3). Realizar comentarios en PDF considerando sintaxis Markdown, por ej. en comentarios crear notas, conceptos o linkear a notas ya existentes con [[ejemplo1]] 

- [ ] **Paso 2** : Subrayar en el PDF con el código AN-RGB (Amarillo, Rojo, Verde, Azul). Hay que modificar propiedades de extract annotations del zotfile, más comentarios en el video de Bri Watson http://zotfile.com/#extract-pdf-annotations
#EstadoArtePI  Amarillo: Comentarios, Estado del Arte
 #CrossrefPI en Naranjo si es Referencia Cruzada 
 #MetodologiasPI Verde: Metodología utilizada
 #ProblemaPI Rojo: Problema o Discusiones presentes en el autor.
#BaseDatosPI Azul: Dato absoluto (edad, PT, litología, coordenada). Extraer tablas con TABULA, luego ir a https://tableconvert.com/ y transformar a MD. 
Figuras interesantes: Se extraen en carpeta **Imágenes y Diagramas PI ** 

- [ ] **Paso 3**: Exportar "batch" incluye 1 archivo con todo (revisar config. en single file) : Metadata y Anotaciones con MDNotes . Esto se exportará a la carpeta Anotaciones Zotero. Seria buena ver una forma de automatizar en la extracción que el color venga como tag. Crear una template para copiar archivos batch.

- [ ] **Paso 4**: Leer notas markdown exportadas a Obsidian. Vienen con sufijo 📃. Asignar #tags y #tags/sub-tags. En la Metadata, asignar como tag el #año de publicación para luego poder filtrar las publicaciones por año. 

- [ ] **Paso 5**: Realizar queries de tematicas importantes. Por ej. Magmatismo-edad. Estos queries van acompañados de notas al pie que sirven de comentarios propios o ideas como backlinks a [[051- Ejemplo Nota Idea]].

- [ ] **Paso 6**: Relectura de [[051- Ejemplo Nota Idea]]. Revisión de queries, depuración de metadata. Luego ingresar nuevo input.

- [ ] **Paso X**: En caso de estar muy cansado, mejor imprimir la publicación, realizar el destacado y comentario en papel. Guardar notas en tu archivador físico y luego traspasar desde el Paso 1 al 6.
- [ ] **Paso 8**: **Búsqueda** 

Ejemplo : tiene una carpeta con información médica y financiera privada llamada “Privada”. Quiere buscar "salud" y no quiere ver resultados ruidosos en sus notas diarias y otras notas aleatorias. Entonces, ya sea en las búsquedas de archivos o en las búsquedas de gráficos, puede simplemente escribir: **`health path:Private`**. ¡Y bum! Recibirá solo los resultados sin ruido de la carpeta Privada :)

Estas son las tres notaciones que debe tener a mano al filtrar carpetas en sus búsquedas:
-   **`path:folder`**
-   **`path:"folder with multiple words"`** \- Usa las comillas así
-   **`-path:folder`**\- Con el signo menos puede excluir carpetas de la búsqueda. Si guarda demasiadas palabras de otras personas, es posible que desee sentirse cómodo con `your_search -path:Sources` , o algo así.

# Para citar en las notas usando Pandoc

 ~~~ 
 pandoc "path/to/input.md" 
 --citeproc --csl 
 "https://raw.githubusercontent.com/citation-style-language/styles/master/apa.csl
 " --bibliography 
 "path/to/citations.bib " -o 
 "path/to/output.docx"
  ~~~ 
  
  just to add if you want to change the citation style, you can choose from here: [https://github.com/citation-style-language/styles](https://github.com/citation-style-language/styles "https://github.com/citation-style-language/styles"), once you have chosen the file, don't forget to chose `Raw`, that's the link you want!
  
  