## Sistemas informáticos
### Ejercicios básicos de MS-DOS

#### Ejercicio 1
> 1. **Crear una estructura de carpetas:**
> 
> ![image](https://user-images.githubusercontent.com/77643882/159536903-d2f84105-e72c-423e-b4a2-a4a9020acfd1.png)
> 
> - Command `MKDIR "dirName0","dirName1"`
> - Command `TREE`

> 2. **Situarse en la carpeta 'TABLAS':**
> 
> ![image](https://user-images.githubusercontent.com/77643882/159545070-17ea55ed-9d7a-4062-8a43-f83b6980bebe.png)
>
> - Command `CD [PATH]`

> 3. **Volver a la carpeta raíz**
> 
> ![image](https://user-images.githubusercontent.com/77643882/159550441-aabc6739-8b65-4698-a3d6-a79a89ca5119.png)
>
> - Command `CD \`

> 4. **Mostrar el contenido de la carpeta 'PROG':**
>
> ![image](https://user-images.githubusercontent.com/77643882/159551524-b40defa5-6a5f-4d49-a00f-f4c76a67e6d2.png)
>
> - Command `CD .\PROG`

> 5. **Borrar la carpeta 'PASCAL'**
> 
> ![image](https://user-images.githubusercontent.com/77643882/159552314-beca5865-64d4-47ab-8cf7-24e59975c982.png)
>
> - Command `RD .\PROG\PASCAL\`

> 6. **Situarse en la carpeta 'VARIOS' y crear una nueva carpeta dentro de 'WORD' llamada 'PRACT':**
> 
> ![image](https://user-images.githubusercontent.com/77643882/159553702-9fdb2393-78b6-4957-877b-0cd5af1d2f31.png)
>
> - Command `MD ..\APLI\WORD\PRACT`

> 7. **Situarse en 'PRACT' y mostrar el contenido de la carpeta 'EXCEL':**
> 
> ![image](https://user-images.githubusercontent.com/77643882/159554561-a5b620b7-712a-41f0-9cda-4891d2c2e3c8.png)
>
> - Command `DIR ..\..\EXCEL\`

> 8. **Desde 'TABLAS' mostrar el listado de archivos y carpetas de la carpeta raíz**
> 
> ![image](https://user-images.githubusercontent.com/77643882/159557825-e063dd69-ff19-4472-9bdd-52e721f8c974.png)
>
> - Command `Get-Childitem -path D:\ -recurse`

> 9. **Situarse en la carpeta 'APLI' y crear una subcarpeta llamada 'Agenda' dentro de 'VARIOS'**
>
> ![image](https://user-images.githubusercontent.com/77643882/159559292-812f322d-aa86-49bc-ae71-7bfdc0962230.png)
>
> - Command `CD .\APLI\` & `MD ..\VARIOS\AGENDA`

> 10. **Borrar la carpeta 'EXCEL':**
>
> ![image](https://user-images.githubusercontent.com/77643882/159561418-8ceb74a8-897d-435d-8e17-805a00dab25b.png)
> 
> - Command `remove-item .\APLI\EXCEL\ -RECURSE`

> 11. **Desde la carpeta raíz, crear una subcarpeta llamada 'NUEVO':**
>
> ![image](https://user-images.githubusercontent.com/77643882/159562153-94a22379-10b9-473e-a205-1c7a5c82c755.png)
> 
> - Command `MD NUEVO`

> 12. **Desde 'PRACT' mostrar el contenido de 'WORD':**
> 
> ![image](https://user-images.githubusercontent.com/77643882/159564591-572d2b3a-6a5b-4f6d-b507-7047a179a82b.png)
>
> - Commands `Set-location .\APLI\WORD\PRACT\` & `Get-childitem ..\`

#### Ejercicio 2
> 
> *Partición nueva (F:) de la unidad (D:)*
>
> 1. **Utilizando el editor de textos de MS-DOS, crear archivo de texto denominado EJER.TXT, con el siguiente contenido, y almacenarlo dentro de la carpeta 'TEXTOS'**
> 
> ![image](https://user-images.githubusercontent.com/77643882/159903030-9962672d-2342-4195-a7b9-d7b4b61b080e.png)
>
> - Commands `NOTEPAD .\APLI\WORD\TEXTOS\EJER.TXT` & `GET-CONTENT .\APLI\WORD\TEXTOS\EJER.TXT` 
>
> 2. **Copiar el archivo 'EJER.TXT' en 'AGENDA':**
>
> ![image](https://user-images.githubusercontent.com/77643882/159904512-53888f8d-6893-4eae-b1b1-247709e4cbcc.png)
>
> - Commands `COPY-ITEM .\APLI\WORD\TEXTOS\EJER.TXT .\VARIOS\AGENDA\EJER.TXT` & `GET-CHILDITEM .\VARIOS\AGENDA`

> 3. **Borrar el archivo almacenado en la carpeta 'TEXTOS':**
>
> ![image](https://user-images.githubusercontent.com/77643882/159905814-2d2a371e-5379-420b-8d21-ebe044748278.png)
>
> - Command `REMOVE-ITEM .\APLI\WORD\TEXTOS\EJER.TXT`

> 4. **Añadir el siguiete párrafo al archivo 'EJER.TXT' *'Cada archivo tiene un nombre y una extensión que los distingue del resto de archivos'* :**
>
> ![image](https://user-images.githubusercontent.com/77643882/159907441-6833048b-35a4-4361-b97e-8f1fcdb13e9a.png)
>
> - Command `NOTEPAD .\VARIOS\AGENDA\EJER.TXT` & `GET-CONTENT .\VARIOS\AGENDA\EJER.TXT`

> 5. **Copiar el archivo 'EJER.TXT' en la carpeta 'BASIC':**
>
> ![image](https://user-images.githubusercontent.com/77643882/159908733-21379336-1da1-4182-905b-b3f21f5eed40.png)
> 
> - Command `COPY-ITEM .\VARIOS\AGENDA\EJER.TXT .\PROG\BASIC\EJER.TXT`

> 6. **Cambiar el nombre del archivo almacenado en 'AGENDA' por 'FICHERO.TXT':**
>
> ![image](https://user-images.githubusercontent.com/77643882/159909337-d7a066da-391f-4342-99ef-95fb6c43c74c.png)
>
> - Commands `RENAME-ITEM .\VARIOS\AGENDA\EJER.TXT FICHERO.TXT` & `GET-CHILDITEM .\VARIOS\AGENDA`

> 7. **Mover el archivo 'FICHERO.TXT' a la carpeta 'BASIC':**
>
> ![image](https://user-images.githubusercontent.com/77643882/159910827-b69455ad-665b-4450-8ef2-324656e319d4.png)
>
> - Command `MOVE-ITEM .\VARIOS\AGENDA\FICHERO.TXT .\PROG\BASIC`

> 8. **Abrir el archivo 'EJER.TXT' y borrar la primera frase; Almacenar el nuevo archivo con el nombre 'NUEVO.TXT' dentro de la carpeta 'BASIC':**
>
> ![image](https://user-images.githubusercontent.com/77643882/159911913-68b876ac-cf01-4f75-aa41-9cb82e1062d3.png)
>
> - Commands `NOTEPAD .\PROG\BASIC\EJER.TXT` & `RENAME-ITEM .\PROG\BASIC\EJER.TXT NUEVO.TXT`

> 9. **Copiar el archivo 'NUEVO.TXT' en la carpeta 'NOTAS':**
>
> ![image](https://user-images.githubusercontent.com/77643882/159912606-3c31bb49-0ec4-48fb-911f-9147b96d2ed2.png)
>
> - Command `COPY-ITEM .\PROG\BASIC\NUEVO.TXT .\APLI\WORD\NOTAS`

> 10. **¿Cuántos archivos hay en la carpeta 'BASIC' y 'NOTAS'?:**
>
> ![image](https://user-images.githubusercontent.com/77643882/159913007-13b291a0-4410-4233-aec0-49b59eda8c74.png)
>
> - Commands `GET-CHILDITEM .\PROG\BASIC\` & `GET-CHILDITEM .\APLI\WORD\NOTAS\`

#### Ejercicio 3

> 1. **Borrar la carpeta 'ACCESS' y en su lugar crear una nueva carpeta llamada 'ASTRO':**
>
> ![image](https://user-images.githubusercontent.com/77643882/159915128-1b03a972-dead-458f-af3c-76e1cd7dc1e3.png)
>
> - Commands `REMOVE-ITEM .\APLI\ACCESS\` & `NEW-ITEM .\APLI\ASTRO -ItemType Directory`

> 2. **Crear una estructura de subcarpetas dentro de la carpeta 'ASTRO':**
>
> ![image](https://user-images.githubusercontent.com/77643882/159925818-0311aaee-4180-4449-a0c4-5d2c1c4673cc.png)
>
> - Commands `MD "HISTORIA","CIENCIA"` & `TREE`

> 3. **Situarse en la carpeta 'CIENCIA' y mostrar el listado de archivos y subcarpetas de la carpeta 'HISTORIA':**
>
> ![image](https://user-images.githubusercontent.com/77643882/159927999-f072bcef-bfba-4e14-9754-b4ec5278370a.png)
>
> - Command `GET-CHILDITEM -recurse ..\HISTORIA\`

> 4. **Utilizar el editor de MS-DOS para crear el siguiente archivo de texto y guardarlo con el nombre 'TYCHO.TXT' dentro de la carpeta 'DATOS1':**
>
> ![image](https://user-images.githubusercontent.com/77643882/159929080-98f4a312-23e0-4763-bb54-ff4256fbd7dd.png)
>
> 
>
>
>
>
>
>
>
>
>
>
>
>
>
>
>
