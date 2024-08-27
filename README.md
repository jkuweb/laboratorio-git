Objetivos

1. Crear un repositorio en local

    - Abre tu terminal y navega hasta el directorio donde deseas crear el repositorio.
    - Crea una carpeta con el nombre del repositorio.<br/>
    - Ingresa a la carpeta que acabas de crear.<br/>
    ``` mkcdir laboratorio-git ```
    - Inicializa el repositorio de Git.<br/>
    ``` git init ```

2. Subir el repositorio a GitHub

    - Crea un nuevo repositorio en GitHub.
    - Copia el URL del repositorio que acabas de crear en GitHub
    - Conecta tu repositorio local con el repositorio en GitHub.<br/>
    ``` git remote add origin git@github.com:jkuweb/laboratorio-git.git ```  
    - Verifica que la conexión se haya establecido correctamente.<br/>
    ``` git remote -v ```

3. Hacer un commit y un push

    - Crea un archivo en la carpeta del repositorio.<br/>
    ``` touch index.html ```
    - Añade el archivo al staging.<br/>
    ``` git add index.html  ||  git add . ```
    - Crea un commit con un mensaje descriptivo.<br/>
    ``` git commit -m 'Add html file to the project' ```
    - Sube los cambios al repositorio en GitHub.<br/>
    ``` git puh origin main ```

4. Crear una rama

    - Crea una rama nueva llamada "development".
    - Cambia a la nueva rama.<br/>
    ``` git checkout -b 'development' ```
    - Realiza algunos cambios en el archivo que creaste.
    - Añade y haz un commit con los cambios en la rama "development".<br/>
    ``` git add index.html && git commit -m 'some changes in html file ```
    - Sube los cambios a Github.<br/>
    ``` git push origin development ```

5. Hacer un merge

    - Vuelve a la rama "main".<br/>
    ``` git checkout main ```
    - Haz un merge de la rama "development" a la rama "main".<br/>
    ``` git merge development ```
    - Si no hay conflictos, los cambios realizados en la rama "development" se incorporarán a la rama "main".
    - Hax un push de los cambios al repositorio en GitHub.<br/>
    ``` git push origin main ```
