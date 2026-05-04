# coding-challenges-content

Contenido educativo de [coding-challenges.dev](https://coding-challenges.dev) — lecciones, ejemplos y syllabi para los cursos de TypeScript/JavaScript y Python.

Este repositorio contiene únicamente los archivos de contenido (`.mdx` y `.json`). El código de la plataforma vive en el repo principal.

---

## ¿Encontraste algo para mejorar?

Si leyendo una lección notás cualquiera de estas cosas, **tu PR es bienvenido**:

- Un error tipográfico o gramatical
- Un ejemplo de código que no funciona o que se puede simplificar
- Una explicación confusa que se puede redactar mejor
- Información desactualizada (una API cambió, una sintaxis quedó deprecada, etc.)
- Un concepto que falta o que merece más desarrollo
- Un título o descripción del capítulo/lección que no es preciso
- Todo lo que ayude, es bienvenido.

No hace falta que el cambio sea grande. Corregir una sola palabra ya mejora la experiencia de miles de personas.

---

## Estructura

```
├── python/
│   ├── syllabus.json          # orden y metadatos de los capítulos
│   └── *.mdx                  # una lección por archivo
└── typescript/
    ├── syllabus.json
    └── *.mdx
```

Cada archivo `.mdx` corresponde a una lección. El nombre del archivo es el `slug` que aparece en la URL: `/learn/typescript/variables` → `typescript/variables.mdx`.

---

## Cómo contribuir

1. **Hacé un fork** de este repositorio.
2. **Editá** el archivo `.mdx` o `.json` que querés mejorar.
3. **Abrí un Pull Request** describiendo qué cambiaste y por qué.

No necesitás instalar nada. Los archivos son texto plano — podés editarlos directo desde GitHub si el cambio es pequeño.

### Frontmatter de las lecciones

Cada `.mdx` empieza con un bloque de metadatos:

```yaml
---
title: 'Título completo de la lección'
short: 'Título corto para la barra lateral'
chapter: '02'
num: '03'
chapterTitle: 'Sintaxis'
difficulty: beginner | intermediate | advanced
readingMinutes: 8
appliesTo: [js, ts] # o [py] para Python
lede: 'Una frase que resume de qué trata la lección.'
---
```

Si modificás el contenido de un `.mdx` no es necesario tocar el frontmatter. Solo cambialo si el título o la descripción es lo que querés corregir.

### Componentes disponibles en MDX

Las lecciones pueden usar estos componentes sin importarlos (están disponibles globalmente):

| Componente                                   | Uso                                        |
| -------------------------------------------- | ------------------------------------------ |
| `<Section title="...">`                      | Agrupa contenido en una sección con título |
| `<CodeBlock tabs={[{lang, label, code}]} />` | Bloque de código con pestañas por lenguaje |
| `<Callout type="tip\|warning\|info">`        | Caja de aviso o consejo                    |
| `<CompareTable>`                             | Tabla comparativa de dos columnas          |
| `<Rules>` / `<Rule>`                         | Lista de reglas o buenas prácticas         |
| `<KeywordPill>`                              | Píldora inline para destacar una keyword   |

---

## ¿Dudas?

Abrí un [issue](../../issues) y lo vemos. Toda pregunta es válida.

Gracias por tomarte el tiempo de mejorar el contenido. 🙌
