# Editor de Imágenes con Álgebra Matricial

**Fundamentos de Álgebra - Unidad III: Álgebra Lineal Aplicada**  
Tecnológico de Software

# Actividad 17: Editor de imágenes matricial

## 👨‍💻 Información del Estudiante

- **Nombre:** [Ángela Yaritzi Rojas Brito]
- **Matrícula:** [SW2509026]
- **Grupo:** [B]
- **Cuatrimestre:** Primer Cuatrimestre
- **Carrera:** TSU en Desarrollo e Innovación de Software
- **Profesor:** Jorge Javier Pedrozo Romero


---

## 📋 Descripción del Proyecto

Este repositorio contiene mi solución a la práctica de **Fundamentos de Programación**, donde implemento funciones en JavaScript para resolver problemas de álgebra básica, preparándome para trabajar con operaciones matriciales más complejas.

## 🎯 Objetivos Alcanzados

- ✅ Dominar variables y tipos de datos en JavaScript
- ✅ Implementar estructuras condicionales
- ✅ Utilizar bucles y funciones
- ✅ Manipular arrays unidimensionales
- ✅ Trabajar con arrays bidimensionales (matrices)
- ✅ Aplicar control de versiones con Git y GitHub

---

## 📊 Progreso de Ejercicios

### Sección 1: Fundamentos (20 puntos)

Conversión entre imágenes y matrices

- [x] 1.1 Cargar imagen PNG y convertir a matriz de píxeles (5 puntos) ✅
- [x] 1.2 Convertir matriz de píxeles a imagen PNG (5 puntos) ✅
- [x] 1.3 Obtener un canal específico de color (5 puntos) ✅
- [x] 1.4 Obtener dimensiones de una imagen (5 puntos) ✅

**Puntos obtenidos: 20/20**

### Sección 2: Operaciones básicas (25 puntos)
Aplicar álgebra matricial a píxeles

- [x] 2.1 Ajustar brillo (8 puntos) ✅
- [x] 2.2 Invertir colores (8 puntos) ✅
- [x] 2.3 Convertir a escala de grises (9 puntos) ✅

**Puntos obtenidos: 25/25**

### Sección 3: Transformaciones geométricas (30 puntos)
Aplicar operaciones matriciales para transformar

- [x] 3.1 Voltear horizontal (espejo) (10 puntos) ✅
- [x] 3.2 Voltear vertical (10 puntos) ✅
- [x] 3.3 Rotar 90 grados en sentido horario (10 puntos) ✅

**Puntos obtenidos: 30/30**

### Sección 4: Filtros avanzados (25 puntos)
Operaciones más complejas

- [x] 4.1 Mezclar dos imágenes (8 puntos) ✅
- [x] 4.2 Filtro Sepia (9 puntos) ✅
- [x] 4.3 Detectar bordes (simplificado) (8 puntos) ✅

**Puntos obtenidos: 25/25**

---

## 📈 Calificación Final

```
┌────────────────────────────────────────┐
│  REPORTE DE CALIFICACIÓN               │
├────────────────────────────────────────┤
│  Puntos obtenidos: 100/100             │
│  Porcentaje: 100%                      │
│  🎓 Calificación: A - Excelente        │
└────────────────────────────────────────┘
```

![Tests](../../actions/workflows/test.yml/badge.svg)

---


## 🚀 Instalación y Uso

### Prerrequisitos
- Node.js (versión 14 o superior)
- Git
  
### 1. Clonar el repositorio
```bash
git clone https://github.com/TU-USUARIO/editor-imagenes-matricial.git
cd editor-imagenes-matricial
npm install
```

### Instalar dependencias
```bash
npm install
```

### Ejecutar tests
```bash
npm test
```

### Ejecutar tests en modo watch
```bash
npm run test:watch
```

### Ver cobertura de código
```bash
npm run test:coverage
```

---

## Sistema de Calificación

| Sección | Puntos |
|---------|--------|
| 1. Commits bien documentados | 20 pts |
| 2. README actualizado y personalizado | 25 pts |
| 3. Editor funcional | 30 pts |
| 4. Funciones bien documentadas | 25 pts |
| **TOTAL** | **100 pts** |

---

## 📁 Estructura del Proyecto

```
fundamentos-programacion-practica-1/
│
├── ejercicios.js           # ⭐ Archivo principal con mis soluciones
├── ejercicios.test.js      # Tests automatizados (no modificar)
├── package.json            # Configuración del proyecto
├── README.md               # Este archivo
├── GUIA_ESTUDIANTES.md     # Guía de referencia
├── GUIA_INSTRUCTOR.md      # Guía del profesor
│
└── .github/
    └── workflows/
        └── test.yml        # Configuración de GitHub Actions
```

---

## 💡 Aprendizajes Clave

### Lo que más me costó
- **Ejercicio 2.2 (Invertir colores)**: Me enredé un poco entendiendo cómo aplicar 255 - valor a cada canal sin tocar el alpha.
- **Ejercicio 2.1 (Ajustar brillo)**: Me costó entender bien cómo el factor hacía la imagen más clara u oscura y recordar limitar los valores para que no se pasaran.
  
### Lo que más me gustó
- **Trabajar con píxeles**: Me sorprendió ver cómo pequeños cambios en números hacen que la imagen se vea totalmente diferente.
- **Probar filtros**: Fue entretenido aplicar escala de grises, sepia o mezcla y ver cómo se transformaba todo.
  
### Técnicas aplicadas
- Uso de `for` loops para iteraciones
- Operador módulo `%` para determinar paridad
- Arrays dinámicos con `.push()`
- Bucles anidados para matrices

---

## 🔧 Ejemplos de Código

### Función Favorita: Invertir Colores
```javascript
function invertirColores(matriz) {
  const resultado = [];

  for (let y = 0; y < matriz.length; y++) {
    const filaN = [];

    for (let x = 0; x < matriz[y].length; x++) {
      const px = matriz[y][x];

      filaN.push({
        r: 255 - px.r,
        g: 255 - px.g,
        b: 255 - px.b,
        a: px.a 
      });
    }

    resultado.push(filaN);
  }

  return resultado;
}
```

**Por qué me gusta:** Es una función muy visual: toma los colores y los convierte en su “opuesto”, como si crearas una versión negativa de una foto.

---

## 📚 Recursos Utilizados

- [MDN Web Docs - JavaScript](https://developer.mozilla.org/es/docs/Web/JavaScript)
- [JavaScript.info](https://es.javascript.info/)
- [Stack Overflow](https://stackoverflow.com)
- Guía del estudiante incluida en el repositorio

---

## 🎯 Próximos Pasos

Este proyecto me prepara para:
- ✨ Operaciones matriciales avanzadas (multiplicación, determinantes)
- 🖼️ Desarrollo de editores de imágenes
- 🔐 Implementación de algoritmos de encriptación
- 📊 Creación de calculadoras científicas

---

## 📝 Historial de Commits

```bash
# Ver mi historial completo
git log --oneline --graph --decorate
```

**Commits destacados:**
- `feat: Completar Sección 1 - Variables y tipos de datos`
- `feat: Implementar ejercicios de condicionales`
- `feat: Resolver funciones y bucles`
- `feat: Completar manipulación de arrays`
- `feat: Finalizar arrays bidimensionales - matrices`
- `docs: Actualizar README con resultados finales`

---

## 🤝 Agradecimientos

- **Profesor Jorge Javier Pedrozo Romero** por la estructura del curso y la práctica
- **Compañeros del Grupo [B/C]** por el apoyo mutuo
- **Tecnológico de Software** por la formación integral

---

## 📧 Contacto

- **Email Institucional:** [angela.rojas@tecdesoftware.edu.mx]
- **GitHub:** [angela-rojas05](https://github.com/angela-rojas05)

---

## 📄 Licencia

Este proyecto es parte de las actividades académicas del **Tecnológico de Software** y está bajo la licencia MIT.

---

<div align="center">

**⭐ Si te gustó este proyecto, dale una estrella ⭐**

Hecho con 💙 por [Tu Nombre] - 2025

</div>
