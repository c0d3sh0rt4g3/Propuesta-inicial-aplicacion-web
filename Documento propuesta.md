# Growl

### Índice

1. [Idea de la aplicación](#idea-de-la-aplicación)
2. [Público objetivo](#público-objetivo)
3. [Análisis de mercado](#análisis-de-mercado)
4. [Funcionalidades clave](#funcionalidades-clave)
5. [Tecnologías seleccionadas](#tecnologías-seleccionadas)

### Idea de la aplicación

Growl es una aplicación de recetas que, aparte de mostrar las recetas en sí, permite filtarlas por aspectos como los 
alérgenos o los valores nutricionales de estos platos.

### Público objetivo

El público objetivo de la aplicación son personas que tengan algún tipo de alergia asi como personas que busquen comer 
saludable controlando, por ejemplo, su ingesta de calorías en sus comidas.

### Análisis de mercado

Actualmente, ya existen webs y aplicaciones como [AllRecipes](https://www.allrecipes.com/) o 
[The real food dietitians](https://therealfooddietitians.com/recipe-filter/) que permiten buscar según los valores 
nutricionales de las recetas asi como webs y aplicaciones como [The allergy chef](https://raise.theallergychef.com/advanced-recipe-search/) 
o [Allergy force](https://www.allergyforce.com/) que las filtran según los alérgenos, 
sin embargo, no existe ninguna web que permita filtrar ambos y además, simultáneamente sin necesidad de especificar 
además un tipo de dieta en concreto.

### Funcionalidades clave

La funcionalidad clave y principal de la aplicación es el filtrado de recetas segun valores nutricionales y alérgenos, 
ademas, la página permitirá crearse una cuenta, esta cuenta nos permitirá tener nuestras alergias en nuestro perfil, 
para que se marquen de manera automática a la hora de buscar recetas, haciendo las búsquedas más cómodas, a su vez, con 
la cuenta también se podrán añadir recetas a favoritos con 1 solo click.

### Tecnologías seleccionadas

Como tecnologías a usar he decidido realizar la parte del cliente con react, puesto que es simple de utilizar, 
es ligero y además su documentación es fácil de entender y bastante intuitiva, para el apartado del diseño, utilizaré 
Sass puesto que ofrece mas facilidades que CSS a la hora de trabajar en un proyecto, ofreciendo funcionalidades como los 
mixings, las variables y la herencia, por último, para la parte del servidor he decidido utilizar Springboot puesto que 
considero que usando este framework, aspectos como la gestión de la base de datos de los usuarios, podrían ser realizados
de manera eficaz sin llegar a cargar la aplicación en exceso.