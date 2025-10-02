# modulo2_Interfaz
# Proyecto Gestor de Usuarios en Java Swing

## Descripcion
Este es un trabajo de la asignatura donde teniamos que hacer una interfaz grafica con **paneles y layouts**.  
Yo lo llame como "Gestor de Usuarios" porque la profe pidio que tuviera un formulario en el centro, un menu a la izquierda, unas pestañas a la derecha y botones abajo.  
No es un proyecto gigante pero me sirvio para practicar como usar BorderLayout, FlowLayout y GridLayout en la misma ventana.

---

## Estructura de la app
La ventana principal la hice con **BorderLayout** y cada parte es asi:

- **Arriba (NORTH)**: un panel con FlowLayout donde puse el logo de AlfonsiFY y un JLabel con el titulo "Gestor de usuarios".  
- **Izquierda (WEST)**: un panel con GridLayout(5x1) que son 5 botones: Menu, Usuarios, Informes, Ajustes y Ayuda.  
- **Centro (CENTER)**: el formulario con GridLayout(5x2). Aqui puse: Nombre, Email, Rol (un comboBox), Activo (un checkBox) y Notas (un JTextArea con scroll).  
- **Derecha (EAST)**: un panel con un JTabbedPane. Hice dos pestañas: "Logs" (con un JTextArea para mostrar mensajes de ejemplo) y "Resumen" (otro JTextArea pero solo lectura).  
- **Abajo (SOUTH)**: la botonera con FlowLayout(RIGHT), con Cancelar, Limpiar y Guardar.  

---

## Cosas que probe
- Los campos de texto se estiran cuando agrandas la ventana.  
- El area de Notas tambien crece (vertical y horizontal).  
- El panel de la derecha (Logs/Resumen) se mantiene con un ancho fijo.  
- La botonera siempre se queda alineada a la derecha.  
- El boton Guardar abre un **JDialog modal** que pregunta si quieres guardar los cambios.  

---

## Como ejecutar
1. Abrir el proyecto en IntelliJ IDEA.  
2. Ejecutar la clase **Main.java**.  
3. Se abre la ventana principal.  

Tambien se puede compilar y correr desde terminal si se quiere, con algo asi (si estas en la carpeta bin):  
```bash
java abuela.Main
