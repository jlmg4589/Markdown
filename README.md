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

### **1.2.3 Resaltar un comando**
**Sintaxis Markdown:**  
En esta frase estamos resaltando el comando \`ls -la\`.  
**HTML renderizado en GitHub:**  
En esta frase estamos resaltado el comando `ls -la`.  


### **1.2.4 Bloques de código**  
Al inicio del bloque se puede indicar de forma opcional cuál es el tipo de contenido que contiene el bloque para resaltar las palabras reservadas cuando se renderice. Por ejemplo: `bash`, `python`, `yaml`, `json`, `html`, `javascript`, etc.  
**Sintaxis Markdown:**  

\`\`\`  
sudo systemctl start apache2  
\`\`\`  

\`\`\`bash  
#!/bin/bash  
echo "Hola mundo"  
\`\`\`

\`\`\`python  
celsius = float(input('Introduce una temperatura en grados Celsius: '))  
farenheit = (1.8 * celsius) + 32  
print(f'La temperatura en grados Farenheit es: {farenheit}')  
\`\`\`

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

Esta forma de gestionar los enlaces puede ser útil cuando vamos a utilizar el mismo enlace varias veces en el documento.

### 1.2.6 Imágenes  

**Sintaxis Markdown:**  

```  
![](https://pro.iesdonana.org/assets/logo.png "Leyenda de la imagen")
```  

```  
![](/images/instituto.jpeg)
```  


**HTML renderizado en GitHub:**  

![|10](https://pro.iesdonana.org/assets/logo.png)  

![](/images/instituto.jpeg)


















[1]: https://iesdonana.org
[2]: https://github.com

