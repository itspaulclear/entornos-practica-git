## Agregar un archivo a un repositorio de Github 💻

### 1. Método tradicional
> Se podrá realizar tanto con *Símbolo del sistema* como con *Git Bash* y se asume que el repositorio se encuentra enlazado con la cuenta personal del usuario.

- Crea una carpeta para ubicar los archivos que se desean incluir dentro del repositorio local.

    - **Forma manual**: haz clic derecho sobre el área del escritorio para seleccionar la opción de *crear carpeta* e introduce cualquier nombre <ins>(resultará indiferente de cara al usuario)</ins>.
    - **Forma automática**: Se deberá inicializar cualquiera de los softwares mencionados previamente <ins>(descarga la *suite* de **[Git](https://git-scm.com/downloads "Suite de Git")**)</ins> e introducir el siguiente comando:

        ~~~
        mkdir NombreDeCarpeta
        ~~~
- Introduce dentro de la carpeta los archivos que tendrán nombres diferentes para evitar cualquier imprevisto surgido en el proceso de subida.
    - **Forma manual**: copie los documentos para posteriormente pegarlos dentro de la carpeta recientemente creada. 
    - **Forma automática**: diríjase al directorio donde se encuentran los archivos, cópielos e introduzcalos en la nueva carpeta. Utilice los siguientes comandos:
        - Acceso a la carpeta:
            ~~~
            cd nombreDecarpeta 
            cd .. /* Regresar al directorio general */
            ~~~
        - Copiar los archivos <ins>(e.g.: se seleccionará el *archivo1* para ser insertado dentro del directorio *d1*)</ins>:

            ~~~
            copy archivo1.txt d1
            ~~~
- Se deberá ubicar dentro de la nueva carpeta e introducir la abreviatura *cmd* en la barra de búsqueda del explorador de archivos o abrir *Git Bash* para localizar el directorio.

    | Símbolo del sistema | Git Bash |
    |---------------------|----------|
    |![cmd](/img/ExploradorArchivos.jpg "cmd") | ![Git Bash](/img/GitBash.png "Git Bash") |
- Deberá iniciar el software de *Git* introduciendo el siguiente comando:
    ~~~
    git init
    ~~~
- Se dispondrá de la opción de añadir todos los archivos contenidos dentro de la carpeta a la cola de subida o seleccionar los ficheros individualmente con el comando:
    ~~~
    git add . /* Se seleccionarán todos los archivos */
    git add nombreDelArchivo
    ~~~
- Se deberá realizar un *commit* para guardar todos los cambios realizados, además de añadirse una breve descripción con el siguiente comando:
    ~~~
    git commit -m "mensaje"
    ~~~
- Se subirán los *commits* desde el repositorio *git* local al repositorio remoto.
    ~~~
    git push -u origin main 
    ~~~
### 1.1. Comandos empleados
| **Generales** | ***Git*** |
|-----------|-----|
| ![Comandos generales](/img/ComandosGenerales.png "Comandos Generales") | ![Comandos Git](/img/ComandosGit.png "Comandos Git") |

### 2. Método alternativo
- Acceda a la web de [Github](https://github.com/) y regístrese para poder crear su primer repositorio haciendo clic en ***Sign up*** o inicie sesión con la opción de ***Sign in***.

    ![Landing Page](/img/LandingPage.png)
- Seleccione el menú desplegable ***Add file*** que se sitúa encima de la lista de archivos de su perfil y haga clic en ***Upload files***. Así mismo, dispone de la opción de arrastrar y colocar los archivos en el explorador.

    ![Seleccionar archivos](/img/Alternativo.png)
- Escriba un mensaje de confirmación breve y aclarativo para describir el archivo que desea subir a su repositorio. 
- Debajo de los campos para el mensaje de confirmación, decide si deseas agregar tu confirmación a la rama actual o a una rama nueva. 
    - Se debe elegir <ins> Create a new branch for this commit and start a pull request</ins> si su rama actual es la rama predeterminada y realizar la subida pulsando sobre <ins>Propose changes</ins>.

        ![Commit](/img/Commit.png)
#### *Sígame en mis otras redes sociales para mantenerse actualizado de próximos tutoriales:*
[![Linkedin](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white
)](www.linkedin.com/in/pablo-garcía-rodríguez-3ba9992b2)
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white
)](<a href="mailto:pagarov@gmail.com?Subject=Interesado%20en%20el%20curso">)

