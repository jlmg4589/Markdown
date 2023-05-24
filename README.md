# **1 Taller de introducción a Markdown**  
## **1.1 ¿Qué es Markdown?**  
[Markdown](https://daringfireball.net/projects/markdown/) es un lenguaje de marcado ligero creado por [John Gruber](https://en.wikipedia.org/wiki/John_Gruber) y [Aaron Swartz](https://es.wikipedia.org/wiki/Aaron_Swartz) que trata de **facilitar la redacción y lectura de documentos en texto plano**, utilizando un conjunto de etiquetas muy sencillas para aplicar estilo al documento.

Actualmente no existe un estándar para Markdown, por este motivo existen diferentes versiones o flavors de Markdown.

En este curso vamos a trabajar con el flavor que se utiliza en GitHub para redactar los archivos README.md de los repositorios y la documentación técnica de los proyectos.

## **1.2 Etiquetas básicas de Markdown**
### **1.2.1 Encabezados**
**Sintaxis Markdown:**

```
# Esto es un ecabezado h1
## Esto es un encabezado h2
### Esto es un encabezado h3
#### Esto es un encabezado h4
##### Esto es un encabezado h5
###### Esto es un encabezado h6
```

**HTML renderizado en GitHub:**

# Esto es un ecabezado h1
## Esto es un encabezado h2
### Esto es un encabezado h3
#### Esto es un encabezado h4
##### Esto es un encabezado h5
###### Esto es un encabezado h6

### **1.2.2 Negrita y cursiva**
| **Estilo** | **Sintaxis** | **Ejemplo** | **Salida**  
| --- | --- | --- | ---
| Negrita | ** ** o __ __ | \*\*Texto en negrita\*\* | **Texto en negrita**
| Cursiva | * * o _ _ | \*Texto en cursuva\*| *Texto en cursiva*
| Tachado | \~\~ \~\~ | \~Texto tachado\~ | ~~Texto tachado~~

### **1.2.3 Resaltar un comando**
**Sintaxis Markdown:**  
En esta frase estamos resaltando el comando \`ls -la\`.  
**HTML renderizado en GitHub:**  
En esta frase estamos resaltado el comando `ls -la`.  


### **1.2.4 Bloques de código**  
Al inicio del bloque se puede indicar de forma opcional cuál es el tipo de contenido que contiene el bloque para resaltar las palabras reservadas cuando se renderice. Por ejemplo: `bash`, `python`, `yaml`, `json`, `html`, `javascript`, etc.  
**Sintaxis Markdown:**  


````
```
sudo systemctl start apache2
```
````

````
```bash  
#!/bin/bash  
echo "Hola mundo"  
```
````
````
```python  
celsius = float(input('Introduce una temperatura en grados Celsius: '))  
farenheit = (1.8 * celsius) + 32  
print(f'La temperatura en grados Farenheit es: {farenheit}')  
```
````

**HTML renderizado en GitHub:**  

```
sudo systemctl start apache2
```

```bash
#!/bin/bash
echo "Hola mundo"
```

```python
celsius = float(input('Introduce una temperatura en grados Celsius: '))
farenheit = (1.8 * celsius) + 32
print(f'La temperatura en grados Farenheit es: {farenheit}')
```

###  Enlaces  

**Sintaxis Markdown:**  
```  
[Enlace a la página web del IES Doñana](https://iesdonana.org)  
```

**HTML renderizado en GitHub:**  

[Enlace a la página web del IES Doñana](https://iesdonana.org)  

#### **1.2.5.1 Otra forma de gestionar enlaces**

También se pueden crear enlaces con esta sintaxis:

**Sintaxis Markdown:**  
```  
Enlaces a la página web del [IES Donñana][1] y a [GitHub][2].

[1]: https://iesdonana.org
[2]: https://github.com
```  

**HTML renderizado en GitHub:**  

Enlaces a la página web del [IES Donñana][1] y a [GitHub][2].

[1]: https://iesdonana.org
[2]: https://github.com

Esta forma de gestionar los enlaces puede ser útil cuando vamos a utilizar el mismo enlace varias veces en el documento.  

### **1.2.6 Imágenes**  

**Sintaxis Markdown:**  

```markdown
Markdown:
![imagen1](https://pro.iesdonana.org/assets/logo.png "Leyenda de la imagen")
```  

```html
HTML:  
<p align="center">
    <img src="https://pro.iesdonana.org/assets/logo.png" alt="JuveR" width="300px">
</p>
```

```markdown
Markdown:
![imagen3](/images/instituto1.jpeg)
```  

**HTML renderizado en GitHub:**  

![](https://pro.iesdonana.org/assets/logo.png)

<p align="center">
    <img src="https://pro.iesdonana.org/assets/logo.png" alt="JuveR" width="300px">
</p>

![imagen3](/images/instituto1.jpg)

### **1.2.7 Listas**
**Sintaxis Markdown:**  
```
* Item 1
* Item 2
* Item 3
* Item 4
```

**HTML renderizado en GitHub:**  

* Item 1
* Item 2
* Item 3
* Item 4

#### **1.2.7.2 Listas desordenadas anidadas**
**Sintaxis Markdown:**  
```
* Item 1
    * Item 1.1
    * Item 1.2
* Item 2
    * Item 2.1
* Item 3
* Item 4
```
**HTML renderizado en GitHub:**  

* Item 1
    * Item 1.1
    * Item 1.2
* Item 2
    * Item 2.1
* Item 3
* Item 4

#### **1.2.7.3 Listas ordenadas**
**Sintaxis Markdown:**  
```
1. Item 1
2. Item 2
3. Item 3
4. Item 4
```

**HTML renderizado en GitHub:**  
1. Item 1
2. Item 2
3. Item 3
4. Item 4

#### **1.2.7.4 Listas ornenadas anidadas**
**Sintaxis Markdown:** 

```
1. Item 1
    1.1 Item 1.1
    1.2 Item 1.2
2. Item 2
    2.1 Item 2.1
3. Item 3
4. Item 4
```
**HTML renderizado en GitHub:** 

1. Item 1  
    1.1 Item 1.1  
    1.2 Item 1.2  
2. Item 2  
    2.1 Item 2.1  
3. Item 3  
4. Item 4  




#### **1.2.7.5 Listas de comprobación**
**Sintaxis Markdown:** 
```
- [x] Caso 1  
- [ ] Caso 2
- [ ] Caso 3
- [x] Caso 4
```
**HTML renderizado en GitHub:** 

- [x] Caso 1  
- [ ] Caso 2
- [ ] Caso 3
- [x] Caso 4

### **1.2.8 Tablas**
**Sintaxis Markdown:** 
```
| Encabezado 1 | Encabezado 2 | Encabezado 3
| --- | --- | --- | ---
| Fila 1.1 | Fila 1.2 | Fila 1.3
| Fila 2.1 | Fila 2.2 | Fila 2.3
| Fila 3.1 | Fila 3.2 | Fila 3.3
```
**HTML renderizado en GitHub:** 

| **Encabezado 1** | ***Encabezado 2*** | **Encabezado 3**  
| --- | --- | ---   
| *Fila 1.1* | Fila 1.2 | Fila 1.3  
| Fila 2.1 | *Fila 2.2* | Fila 2.3  
| Fila 3.1 | Fila 3.2 | *Fila 3.3*  

### **1.2.9 Forzar un salto de línea**  
Para forzar un salto de línea es necesario incluir dos espacios en blanco y un salto de línea.

**Sintaxis Markdown:**  
```
Por ejemplo, en esta frase  
hemos forzado un salto de línea.
```

**HTML renderizado en GitHub:**  

Por ejemplo, en esta frase  
hemos forzado un salto de línea.

### **1.2.10 Citar textos**
**Sintaxis Markdown:**  
```
Este texto no es una cita.
> Este texto daría como resultado una cita.
```

**HTML renderizado en GitHub:**  

Este texto no es una cita.
> Este texto daría como resultado una cita.

### **1.2.11 Comentarios**  
Para poner un comentario en Markdown y que su contenido no sea rendereizado, se utiliza la misma sintaxis que los comentarios de HTML.
**Sintaxis Markdown:**  

```
Párrafo 1.


<!-- Este texto es un comentario y no será renderizado -->

Párrafo 2.
```

**HTML renderizado en GitHub:**  

Párrafo 1.

<!-- Este texto es un comentario y no será renderizado -->

Párrafo 2.

### **1.2.12 Diagrama de flujo**

**HTML renderizado en GitHub:**  


````
Simple diagrama de flujo:

```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```
````

**HTML renderizado en GitHub:**  

Simple diagrama de flujo:

```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```

[Editor de mermaid](https://mermaid.live)


### **1.2.14 Ecuaciones matemáticas**
**HTML renderizado en GitHub:**  
Para habilitar una comunicación clara de las expresiones matemáticas, GitHub admite expresiones matemáticas con formato LaTeX en Markdown.  
Como ya se ha comentado, al igual que ocurre con Latex, para poner una ecuación se ha de poner entre $ la expresión concreta.

* Para insertar una ecuación dentro de una frase, o para utilizar un carácter especial, como letras griegas.
```
La ecuación, $x=\frac{-b \pm \sqrt{{b}^{2} - 4 \cdot a \cdot c}}{2 \cdot a}$, es de segundo grado.
```

* Como bloque.
```
La ecuación de segundo grado es:
$$x=\frac{-b \pm \sqrt{{b}^{2} - 4 \cdot a \cdot c}}{2 \cdot a}$$
```


**HTML renderizado en GitHub:**  

* Dentro de una frase:  
La ecuación, $x=\frac{-b \pm \sqrt{{b}^{2} - 4 \cdot a \cdot c}}{2 \cdot a}$, es de segundo grado.

* En un bloque.  
La ecuación de segundo grado es:  
$$x=\frac{-b \pm \sqrt{{b}^{2} - 4 \cdot a \cdot c}}{2 \cdot a}$$

[Editor de ecuacione para Latex](https://latex.codecogs.com/eqneditor/editor.php?lang=es-es)

