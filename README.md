# holamundo-pyside6

Documentación y código para una aplicación simple de PySide6 "Hola Mundo".

## Hola Mundo PySide6

Esta es una aplicación simple "Hola Mundo" creada con **PySide6**. A continuación, encontrarás las instrucciones para instalar y ejecutar la aplicación en **Windows** y **Linux**.

---

## Instalación

### 1. Instalación de Python3

#### **Windows**

1. Descarga Python3 desde el sitio oficial: [https://www.python.org/downloads/](https://www.python.org/downloads/).
2. Durante la instalación, asegúrate de marcar la opción **"Add Python to PATH"**.
3. Verifica que Python esté instalado correctamente abriendo una terminal (cmd) y ejecutando:
   ```bash
   python --version
   ```

#### **Linux**

1. Abre una terminal y ejecuta:
   ```bash
   sudo apt update
   sudo apt install python3
   ```
2. Verifica que Python esté instalado correctamente ejecutando:
   ```bash
   python3 --version
   ```

---

### 2. Instalación y Activación de pip

`pip` es el gestor de paquetes de Python y debería instalarse junto con Python. Para asegurarte de que `pip` esté instalado correctamente, ejecuta el siguiente comando:

```bash
python -m ensurepip --upgrade
```

Verifica que `pip` esté disponible ejecutando:

```bash
pip --version
```

---

### 3. Creación y Activación de un Entorno Virtual

Es recomendable crear un entorno virtual para mantener las dependencias del proyecto aisladas.

#### **Windows**

1. Abre una terminal (cmd o PowerShell) y navega hasta la carpeta del proyecto.
2. Crea el entorno virtual con el siguiente comando:
   ```bash
   python -m venv venv
   ```
3. Activa el entorno virtual:
   - En **cmd**:
     ```bash
     venv\Scripts\activate
     ```
   - En **PowerShell**:
     ```bash
     .\venv\Scripts\Activate
     ```

#### **Linux**

1. Abre una terminal y navega hasta la carpeta del proyecto.
2. Crea el entorno virtual con el siguiente comando:
   ```bash
   python3 -m venv venv
   ```
3. Activa el entorno virtual:
   ```bash
   source venv/bin/activate
   ```

---

### 4. Instalación de Dependencias

Con el entorno virtual activado, instala la librería `PySide6` ejecutando el siguiente comando:

```bash
pip install pyside6
```

---

### 5. Ejecución de la Aplicación

1. Crea un archivo llamado `main.py` en la carpeta del proyecto y agrega el siguiente código:
   
   ```python
   import sys
   from PySide6.QtWidgets import QApplication, QLabel

   app = QApplication(sys.argv)
   label = QLabel("Hola Mundo!")
   label.show()
   app.exec()
   ```

2. Ejecuta la aplicación con el siguiente comando:

#### **Windows**
```bash
python main.py
```

#### **Linux**
```bash
python3 main.py
```

Deberías ver una ventana emergente con el mensaje **"Hola Mundo!"**.

---

## Notas Adicionales

- Si tienes problemas con `pip` o las dependencias, asegúrate de que tu entorno virtual esté correctamente activado.
- Para salir del entorno virtual en cualquier sistema operativo, simplemente ejecuta:
  ```bash
  deactivate
  ```

---



