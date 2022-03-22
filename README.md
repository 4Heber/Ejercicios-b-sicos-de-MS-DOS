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
>
>
>
> 
>
>
>
