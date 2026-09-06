[[IDENTITY]]
```
/mnt/Datos/Archivos/
```

y las categorías:

```
### **00_inbox** (ACTUA COMO LA CARPETA DONDE ALMACENA TODOS LOS ARCHIVOS SIN ORGANIZAR, ES EL DIRECTORIO DEL CUAL PARTIMOS)


        

### **01_Escuela** (Debe contener unicamente los documentos referentes a las clases o estudio)

- Secundaria_semestre_00
    
    - Soc. de Alumnos (Todos somos parte, MARCA)
        
    - Guias de estudio
        
    - Academico
        
- semestre_01
    
    - inscripcion_y_tramites
        
    - materias (Matematicas)
        

### **02_Personal_y_Tramites** (Documentos mas personales como constancias, curps, actas de nacimiento, Imss etc, así como documentos varios que yo te mencionare)

- inscripcion_y_tramites
    
- finanzas_y_recibos
    
- Varios (Videitos, Pachuco, Catholic edits)
    
- IMSS
    
- identificaciones
    

### **03_Biblioteca** (Actua como contenedor para todos mis libros, tanto generales, como los de la escuela)

- general
    
- escolar
    
    - Saberes
        

### **04_Recursos_y_Media** (Recursos para presentaciones, mis dotfiles, etc)

- audio (Soundtrack, Efectos de sonido)
    
- dotfiles_y_configs (configuración de i3 laptop, Firefox, polybar, kitty, rofi, xfce4, etc.)
    
- imagenes (Ponys, Substacks, Wallpapers, Recursos de diseño, Pfps, Personales)
    

### **05_Fotos** (se autodefine)


```

También:

- Ollama clasifica tomando en cuenta la etiqueta que tiene el archivo, en dado caso de no tener etiqueta (00,01,02,03,04,05) se debe de preguntar
- cómo devuelve su propuesta; en formato de lista, listando cada archivo, y su propuesta de nombre, o moviemiento
- si tiene etiqueta puede ser directamente enviado a esa carpeta, si ademas de eso, se indica el contenido (tipo image, o similar), hacer el movimiento automatico, en caso de ser muchos archivos o haber dudas, notificarme, y esperar mi indicacion
- reglas de nombres; debe seguir la regla (id: 00,01,02,03,04,05, etc, despues la fecha en formato DD-MM-AAAA, luego una pequeña descripcion (si no hay descripcion debe ser usando el tipo de archivo, ej. 01-Formulario matematicas-20-08-2026 o Ej. 03-Pdf-1- 03-09-2026))
- conflictos de nombres;Notificarme inmediatamente
- `dry-run`; si se cumplen todas las especificaciones sin dudas (etiqueta, contenido, y fecha) se omite
- qué nunca debe eliminar.: nunca eliminar archivos NO repetidos

La regla principal:

> **Organizar nunca significa eliminar.**