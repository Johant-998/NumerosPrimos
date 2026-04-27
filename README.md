# Verificador de Números Primos

![Version](https://img.shields.io/badge/versión-2.1-7850ff) ![HTML](https://img.shields.io/badge/HTML-5-e34f26) ![CSS](https://img.shields.io/badge/CSS-3-1572b6) ![JavaScript](https://img.shields.io/badge/JavaScript-ES6-f7df1e)

Aplicativo web para determinar si un número entero es primo o no, con visualización paso a paso del proceso de verificación. Desarrollado con estética dark futurista usando HTML, CSS y JavaScript puros en un único archivo.

---

## Vista previa

El aplicativo presenta una interfaz oscura con cuadrícula de fondo, tipografía técnica y retroalimentación visual dinámica: el color del borde y el orbe de luz cambian según el resultado (verde para primo, rojo para no primo).

---

## Características

- Verificación instantánea al presionar Enter o el botón
- Visualización de todos los divisores probados durante el proceso
- Retroalimentación visual con cambio de colores según el resultado
- Chips de prueba rápida con números de ejemplo
- Validación de entradas inválidas o negativas
- Diseño completamente responsivo
- Sin dependencias externas (solo fuentes de Google Fonts)

---

## Tecnologías

| Tecnología | Uso |
|---|---|
| HTML5 | Estructura del documento |
| CSS3 | Estilos, animaciones y variables de color |
| JavaScript ES6 | Lógica del algoritmo e interactividad |
| Google Fonts | Tipografías Syne y Space Mono |

---

## Algoritmo

El verificador utiliza el método de **criba por divisores hasta la raíz cuadrada**, que es el enfoque más eficiente para verificación individual de primalidad:

```
función esPrimo(n):
  si n < 2  → no es primo
  si n = 2  → es primo
  si n es par → no es primo (divisible entre 2)

  para i desde 3 hasta √n, con paso 2:
    si n % i = 0 → no es primo (se encontró divisor)

  si ninguno divide → es primo
```

La complejidad temporal es **O(√n)**, lo que lo hace eficiente incluso para números grandes.

---

## Uso

1. Descarga el archivo `verificador-primo.html`
2. Ábrelo en cualquier navegador moderno (Chrome, Firefox, Edge, Safari)
3. Ingresa un número entero positivo en el campo de texto
4. Presiona **Enter** o el botón **Verificar número**
5. El resultado aparece con el veredicto y el detalle de los divisores probados

No requiere servidor, instalación ni configuración adicional.

---

## Estructura del proyecto

```
verificador-primo/
│
├── verificador-primo.html    # Aplicativo completo (HTML + CSS + JS)
└── README.md                 # Documentación del proyecto
```

---

## Casos de prueba incluidos

El aplicativo trae botones de prueba rápida con los siguientes números de ejemplo:

| Número | Resultado |
|---|---|
| 0, 1 | No primo (menores que 2) |
| 2, 3, 7, 11, 13, 37, 97, 127 | Primo |
| 25, 100 | No primo |

---

## Autor

**Johan Steven Rodríguez**
Diseñador UX/UI — Especialización en Diseño e Inteligencia Artificial

> Elaborado con asistencia de Inteligencia Artificial (Claude — Anthropic)

---

## Licencia

Proyecto de uso académico y personal. Libre para modificar y distribuir con atribución al autor original.
