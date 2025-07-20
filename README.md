# Records

Esta p\u00e1gina registra las puntuaciones de los eventos **Noche de Juegos** organizados por el Departamento de Espa\u00f1ol de la HKU.

## Tecnolog\u00edas utilizadas
- **HTML** y **CSS** para la estructura y el dise\u00f1o de la p\u00e1gina.
- **JavaScript** para la interactividad.
- **Supabase** como base de datos y backend.

## \u00c1brelo en tu m\u00e1quina
1. Clona este repositorio.
2. Crea un proyecto en [Supabase](https://supabase.com) y copia tu URL y clave an\u00f3nima.
3. Abre `index.html` y reemplaza las variables `SUPABASE_URL` y `SUPABASE_ANON_KEY` con tus datos.
4. Abre la p\u00e1gina en tu navegador.

## Estructura de la base de datos
El proyecto espera dos tablas:

### Tabla `games`
| Columna | Tipo | Descripci\u00f3n |
|---------|------|---------------|
| `id`    | `uuid` (PK) | Identificador del juego |
| `name`  | `text` | Nombre del juego |

### Tabla `scores`
| Columna | Tipo | Descripci\u00f3n |
|---------|------|---------------|
| `id`         | `uuid` (PK) | Identificador del registro |
| `player_name`| `text` | Nombre del jugador |
| `score`      | `integer` | Puntuaci\u00f3n obtenida |
| `game_id`    | `uuid` (FK a games.id) | Juego al que pertenece |
| `created_at` | `timestamp` | Fecha de creaci\u00f3n |

## Caracter\u00edsticas
- Muestra los mejores puntajes por juego.
- Permite a los usuarios a\u00f1adir nuevas puntuaciones mediante un formulario.

## Futuras mejoras
- Validaciones adicionales en el formulario.
- Filtros y ordenamientos personalizados.

