# **Ejercicio de Git: Colaboración en un Repositorio Compartido**

## **Objetivo**
Aprender y practicar el uso de Git en un entorno colaborativo mediante la clonación, modificación, creación de ramas, commits, resolución de conflictos y fusión de cambios en un repositorio compartido.

---

## **Instrucciones**

### **1. Clonar el repositorio**
Antes de empezar, clona este repositorio en tu máquina local con el siguiente comando:

```bash
 git clone https://github.com/usuario/proyecto-clase.git
```

Entra en la carpeta del repositorio:

```bash
 cd proyecto-clase
```

---

### **2. Crear una nueva rama**
Para trabajar en tu propio espacio, crea una nueva rama con tu nombre:

```bash
 git checkout -b tu-nombre
```

Ejemplo:
```bash
 git checkout -b maria-gomez
```

---

### **3. Modificar el archivo y hacer un commit**
Abre el archivo `participantes.txt` y añade tu nombre al final de la lista. Luego, guarda los cambios.

Confirma que Git ha detectado los cambios:
```bash
 git status
```

Añade los cambios al área de preparación:
```bash
 git add participantes.txt
```

Realiza un commit con un mensaje descriptivo:
```bash
 git commit -m "Agregando mi nombre - Maria Gomez"
```

---

### **4. Subir los cambios al repositorio remoto**
Envía tu rama al repositorio en GitHub:
```bash
 git push origin tu-nombre
```

---

### **5. Crear un Pull Request (PR)**
1. Ve a la página del repositorio en GitHub.
2. Haz clic en la pestaña "Pull Requests".
3. Crea un nuevo PR desde tu rama (`tu-nombre`) hacia la rama `main`.
4. Agrega un título y descripción explicando tu cambio.
5. Envía el PR y espera la revisión del profesor o un compañero.

---

### **6. Resolver conflictos (si es necesario)**
Si hay conflictos, Git te lo indicará al intentar hacer el merge. Para resolverlos:

1. Descarga los últimos cambios:
   ```bash
   git pull origin main
   ```
2. Edita manualmente los archivos en conflicto.
3. Después de resolver los conflictos, guarda los archivos y haz un commit:
   ```bash
   git add .
   git commit -m "Resolviendo conflictos en participantes.txt"
   ```
4. Sube los cambios nuevamente:
   ```bash
   git push origin tu-nombre
   ```

---

### **7. Fusionar los cambios en `main`**
Una vez aprobado tu Pull Request, fusiónalo en la rama `main` desde GitHub.

Después de la fusión, actualiza tu copia local:
```bash
 git checkout main
 git pull origin main
```

¡Felicidades! Has completado el ejercicio. 🎉
