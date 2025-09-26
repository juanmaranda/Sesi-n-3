# Documentación del Proyecto: Aplicación Demo con Tkinter

## Descripción General
Este proyecto es una aplicación gráfica desarrollada en **Python** utilizando la librería **Tkinter**.  
Se diseñó como un **MVP (Producto Mínimo Viable)** para demostrar el uso de diferentes componentes gráficos, organización de ventanas y manejo de interacciones básicas (formularios, listas, tablas y canvas).

La aplicación cuenta con un menú principal desde donde se accede a las diferentes ventanas de demostración.

---

## Estructura del Proyecto

```
main.py
win_home.py
win_form.py
win_list.py
win_table.py
win_canvas.py
```

Cada archivo contiene la lógica de una ventana específica de la aplicación.

---

## Archivos y Funcionalidad

### 1. `main.py`
- Es el **punto de entrada** de la aplicación.
- Crea la ventana principal (`Tk`) con un menú de botones para abrir las demás ventanas.
- Opciones disponibles:
  1. Home / Bienvenida
  2. Formulario
  3. Lista (CRUD básico)
  4. Tabla (Treeview con datos de CSV)
  5. Canvas (Dibujo)
  6. Salir

👉 Referencia: [`main.py`](main.py)

---

### 2. `win_home.py`
- Ventana de **bienvenida** al usuario.
- Contiene un mensaje inicial y un botón para mostrar un `messagebox` con información adicional.
- Componentes:
  - `Label`: Texto de bienvenida.
  - `Button`: Mostrar mensaje emergente o cerrar ventana.

👉 Referencia: [`win_home.py`](win_home.py)

---

### 3. `win_form.py`
- Implementa un **formulario simple** con campos de entrada:
  - Nombre
  - Edad
- Incluye validaciones:
  - El nombre no puede estar vacío.
  - La edad debe ser un número entero.
- Permite guardar los datos en un archivo `.txt` mediante un `filedialog`.
- Usa `messagebox` para mostrar errores o confirmación.

👉 Referencia: [`win_form.py`](win_form.py)

---

### 4. `win_list.py`
- Ejemplo de una **lista (CRUD básico)**.
- Funcionalidad:
  - Agregar elementos a la lista.
  - Eliminar elemento seleccionado.
  - Limpiar toda la lista.
- Maneja validaciones mostrando advertencias con `messagebox`.
- Componentes:
  - `Listbox`
  - `Entry`
  - Botones de acción

👉 Referencia: [`win_list.py`](win_list.py)

---

### 5. `win_table.py`
- Muestra una **tabla** con `Treeview` de `ttk`.
- Las columnas (`nombre`, `valor1`, `valor2`) se llenan con datos de un archivo CSV (`data/sample.csv`).
- Si el archivo no existe, muestra un `messagebox` de advertencia.
- Funcionalidad de solo lectura.

👉 Referencia: [`win_table.py`](win_table.py)

---

### 6. `win_canvas.py`
- Ejemplo de un **Canvas** para dibujo gráfico.
- Incluye:
  - Rectángulo
  - Óvalo
  - Línea
  - Texto
- Sirve como demostración básica del uso del `Canvas` de Tkinter.

👉 Referencia: [`win_canvas.py`](win_canvas.py)

---

## Requisitos
- Python 3.x
- Librerías estándar:
  - `tkinter`
  - `csv`
  - `pathlib`

No se requieren dependencias externas.

---

## Ejecución
1. Abrir una terminal en la carpeta del proyecto.
2. Ejecutar el comando:

```bash
python main.py
```

3. Navegar por las opciones disponibles en la ventana principal.

---

## Posibles Mejoras Futuras
- Agregar base de datos para persistencia en lugar de archivos de texto/CSV.
- Mejorar la validación en formularios (edad mínima, formato de texto).
- Agregar estilos personalizados a la interfaz con `ttk.Style`.
- Internacionalización (traducciones).

---

## Autores
Proyecto de ejemplo para demostración con **Tkinter**.
