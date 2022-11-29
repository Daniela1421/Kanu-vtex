# Store Theme Vtex Kanu Pet 

[Kanú Pet](https://www.kanu.pet/) es la página base escogida para clonar utilizando la tecnología VTEX IO, a traves de la plantilla de minimum boilerplate theme. Realizando un diseño responsive de las diferentes vistas de la página. 

## Configuration 

### Paso 1 - Configuración Básica

Ingrese a la [guía de configuración básica](https://developers.vtex.com/vtex-developer-docs/docs/vtex-io-documentation-2-basicsetuptodevelopinvtexio) de VTEX IO y siga los pasos. Al final de la configuración, debe tener instalada la interfaz de línea de comandos de VTEX (Toolbelt) junto con un espacio de trabajo de desarrollador en el que puede trabajar.

### Paso 2 - Clonación del repositorio

Realice la [clonación](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository) de este repositorio en sus archivos locales para poder comenzar a trabajar en el. 
Después, acceda al directorio del repositorio usando su terminal.

### Paso 3 - Editar el Manifest.json

Ingrese en el archivo `manifest.json` y reemplace los valores de `vendor`(nombre de la cuenta en la que está trabajando) y `name`(nombre que desee para su tema). Por ejemplo: .
```
{
  "vendor": "itgloberspartnercl",
  "name": "minimum-theme"
} 
```

Además, verifique que el archivo cuente con los siguientes builders: 

```
  "builders": {
    "assets": "0.x",
    "styles": "2.x",
    "store": "0.x",
    "docs": "0.x"
  }
```

### Paso 4 - Instalar apps necesarias

Para usar Store Framework y trabajar en el tema de su tienda, es necesario tener `vtex.store-sitemap` y `vtex.store` instalados.

Ejecute `vtex list` y compruebe si esas aplicaciones ya están instaladas.

Si no es así, ejecute el siguiente comando para instalarlos: 

```
vtex install vtex.store-sitemap vtex.store -f
```

### Paso 5 - Desinstalar el store-theme predeterminado

Al ejecutar el comando `vtex list`, puede verificar si hay algún tema instalado. 

Con frecuencia `vtex.store-theme` ya se encuentra instalado cuando se inicia el proceso de desarrollo front de la tienda. Por lo tanto, si esto ocurre ejecute el siguiente comando para desinstalarlo: 

```
vtex uninstall vtex.store-theme
```

### Paso 6 - Ejecutar el preview de la tienda

Después de realizar los pasos anteriores, es momento de cargar los cambios que realizó en sus archivos locales ejecutando el comando `vtex link`. Si el proceso se lleva a cabo correctamente deberá ver en su terminal el siguiente mensaje: `App linked successfully`. Luego, ejecute el comando `vtex browse` para abrir una ventana del navegador que tenga su tienda vinculada.

Esto le permitirá ver los cambios aplicados en tiempo real, a través de la cuenta y el espacio de trabajo en el que se encuentre.

## Dependencies

1. Minimum Theme
2. Store GraphQl

## Store Component Apps

1.	"vtex.store": "2.x"
2.	"vtex.store-header": "2.x"
3.	"vtex.store-footer": "2.x"
4.	"vtex.store-components": "3.x"
5.	"vtex.styleguide": "9.x"
6.	"vtex.carousel": "2.x"
7.	"vtex.menu": "2.x"
8.	"vtex.minicart": "2.x"
9.	"vtex.product-details": "1.x"
10.	"vtex.product-kit": "1.x"
11.	"vtex.search-result": "3.x"
12.	"vtex.login": "2.x"
13.	"vtex.my-account": "1.x"
14.	"vtex.flex-layout": "0.x"
15.	"vtex.rich-text": "0.x"
16.	"vtex.store-drawer": "0.x"
17.	"vtex.locale-switcher": "0.x"
18.	"vtex.product-quantity": "1.x"
19.	"vtex.product-identifier": "0.x"
20.	"vtex.product-specification-badges": "0.x"
21.	"vtex.product-review-interfaces": "1.x"
22.	"vtex.telemarketing": "2.x"
23.	"vtex.order-placed": "2.x"
24.	"vtex.stack-layout": "0.x"
25.	"vtex.tab-layout": "0.x"
26.	"vtex.responsive-layout": "0.x"
27.	"vtex.slider-layout": "0.x"
28.	"vtex.iframe": "0.x"
29.	"vtex.breadcrumb": "1.x"
30.	"vtex.sticky-layout": "0.x"
31.	"vtex.add-to-cart-button": "0.x"
32.	"vtex.store-image": "0.x"
33.	"vtex.modal-layout": "0.x"
34.	"vtex.store-link": "0.x"
35.	"vtex.overlay-layout": "0.x"
36.	"vtex.search": "2.x"
37.	"vtex.store-icons": "0.x"
38.	"vtex.disclosure-layout": "1.x"
39.	"vtex.checkout-summary": "0.x"
40.	"vtex.product-list": "0.x"
41.	"vtex.product-price": "1.x"
42.	"vtex.store-newsletter": "1.x"
43.	"vtex.product-specifications": "1.x"

## Custom Apps

1. "itgloberspartnercl.whatsapp-button": "0.x"
2. "itgloberspartnercl.bullets-diagramation": "0.x
3. "itgloberspartnercl.add-to-cart-info": "0.x"
4. "itgloberspartnercl.pdf-reader": "0.x"
5. "itgloberspartnercl.custom-department-search": "0.x"
6. "itgloberspartnercl.quick-order": "0.x"

# Peer Dependencies

1. "vtex.wish-list": "1.x"
2. "vtex.questions-and-answers": "0.x"

## Contributors ✨

Daniela Ducuara Cañas
