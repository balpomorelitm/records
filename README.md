# Records

Esta página registra las puntuaciones de los eventos **Noche de Juegos** organizados por el Departamento de Español de la HKU.

## Tecnologías utilizadas
- **HTML** y **CSS** para la estructura y el disño de la página.
- **JavaScript** para la interactividad.
- **Supabase** como base de datos y backend.


## Estructura de la base de datos
El proyecto espera dos tablas:

### Tabla `games`
| Columna | Tipo | Descripción |
|---------|------|---------------|
| `id`    | `uuid` (PK) | Identificador del juego |
| `name`  | `text` | Nombre del juego |

### Tabla `scores`
| Columna | Tipo | Descripción |
|---------|------|---------------|
| `id`         | `uuid` (PK) | Identificador del registro |
| `player_name`| `text` | Nombre del jugador |
| `score`      | `integer` | Puntuación obtenida |
| `game_id`    | `uuid` (FK a games.id) | Juego al que pertenece |
| `created_at` | `timestamp` | Fecha de creación |

## Caracter\u00edsticas
- Muestra los mejores puntajes por juego.
- Permite a los usuarios añadir nuevas puntuaciones mediante un formulario.

## Futuras mejoras
- Validaciones adicionales en el formulario.
- Filtros y ordenamientos personalizados.

