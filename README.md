# Git tutorial: PAL INGENIERO
### **1. Instalación de Git en la Máquina Local**

Para instalar Git, puedes usar los siguientes comandos dependiendo del sistema operativo:

**Windows:**

- Descarga el instalador desde el sitio oficial de Git: [git-scm.com](https://git-scm.com/)
- Sigue las instrucciones del instalador.

**macOS:**

```bash
brew install git

```

*Nota: Necesitarás tener Homebrew instalado en tu máquina. Si no lo tienes, primero instala Homebrew usando:*

```bash
/bin/bash -c "$(curl -fsSL <https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh>)"

```

**Linux (Debian/Ubuntu):**

```bash
sudo apt update
sudo apt install git

```

Para verificar la instalación:

```bash
git --version

```

---

### **2. Creación de un Repositorio en GitHub**

1. Inicia sesión en GitHub.
2. Haz clic en el botón "New" para crear un nuevo repositorio.
3. Llena los campos "Repository name" y "Description".
4. Selecciona si quieres que el repositorio sea público o privado.
5. Marca las opciones para inicializar con un README, agregar `.gitignore` o elegir una licencia (opcional).
6. Haz clic en "Create repository".

---

### **3. Clonar el Repositorio en Local usando CLI**

Para clonar un repositorio, usa el siguiente comando en la terminal:

```bash
git clone <https://github.com/tu_usuario/tu_repositorio.git>

```

*Reemplaza `tu_usuario` y `tu_repositorio` por el nombre de tu cuenta y repositorio en GitHub.*

---

### **4. Hacer un Commit usando CLI y Extensión**

**CLI:**

1. Haz cambios en tu proyecto.
2. Añade los cambios al staging area:
    
    ```bash
    git add .
    
    ```
    
3. Realiza un commit:
    
    ```bash
    git commit -m "Descripción del commit"
    
    ```
    

**Extensión en VS Code:**

1. Realiza cambios en tu proyecto.
2. Abre la vista de "Source Control" en VS Code.
3. Escribe un mensaje de commit en el campo correspondiente.
4. Haz clic en el ícono de check para confirmar el commit.

---

### **5. Uso de `git commit --amend` para Modificar un Commit**

Si necesitas modificar el último commit:

```bash
git commit --amend -m "Nuevo mensaje del commit"

```

*Este comando reemplaza el mensaje del último commit y te permite agregar cambios adicionales si los hay.*

---

### **6. Hacer Push de Cambios al Repositorio Remoto**

Para subir los cambios al repositorio remoto:

```bash
git push origin main

```

*Nota: Reemplaza `main` con el nombre de tu rama si es diferente.*

---

### **7. Sincronizar Cambios con `git pull`**

Para sincronizar los cambios desde el repositorio remoto:

```bash
git pull origin main

```

*Esto descargará y fusionará los cambios de la rama `main` del repositorio remoto en tu copia local.*

---

### **8. Abrir un Pull Request**

1. Cambia a una nueva rama utilizando el nuevo comando `switch`:
    
    ```bash
    
    git switch -c nombre-de-la-rama
    
    ```
    
    *El comando `switch` es ahora el recomendado para cambiar entre ramas y crear nuevas ramas.*
    
2. Empuja los cambios a la nueva rama:
    
    ```bash
    
    git push origin nombre-de-la-rama
    
    ```
    
3. Ve a GitHub y navega al repositorio.
4. Verás un mensaje para crear un Pull Request (PR) para la nueva rama.
5. Haz clic en "Compare & pull request".
6. Añade un título y descripción para el PR.
7. Haz clic en "Create pull request".