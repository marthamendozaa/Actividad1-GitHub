# - H1 Actividad1-GitHub
# - Martha Mendoza Alfaro
# - ITC
# - Monterrey
## - Equipo -

# **Semana Tec**
😀😆🥹🤣😇🙂

# 2. Tipos de Letra
**bold text**
*italicized text*
> blockquote

# 3. Lista Enumerada
1. Gorditas doña tota
2. Taquitos
3. Corundas

# 4. Lista con viñetas
- First item
- Second item
- Third item

# 5. Código
`code`
```
from turtle import *

from freegames import vector


def line(start, end):
    """Draw line from start to end."""
    up()
    goto(start.x, start.y)
    down()
    goto(end.x, end.y)


def square(start, end):
    """Draw square from start to end."""
    up()
    goto(start.x, start.y)
    down()
    begin_fill()

    for count in range(4):
        forward(end.x - start.x)
        left(90)

    end_fill()


def circle(start, end):
    """Draw circle from start to end."""
    pass  # TODO


def rectangle(start, end):
    """Draw rectangle from start to end."""
    pass  # TODO


def triangle(start, end):
    """Draw triangle from start to end."""
    pass  # TODO


def tap(x, y):
    """Store starting point or draw shape."""
    start = state['start']

    if start is None:
        state['start'] = vector(x, y)
    else:
        shape = state['shape']
        end = vector(x, y)
        shape(start, end)
        state['start'] = None


def store(key, value):
    """Store value in state at key."""
    state[key] = value


state = {'start': None, 'shape': line}
setup(420, 420, 370, 0)
onscreenclick(tap)
listen()
onkey(undo, 'u')
onkey(lambda: color('black'), 'K')
onkey(lambda: color('white'), 'W')
onkey(lambda: color('green'), 'G')
onkey(lambda: color('blue'), 'B')
onkey(lambda: color('red'), 'R')
onkey(lambda: store('shape', line), 'l')
onkey(lambda: store('shape', square), 's')
onkey(lambda: store('shape', circle), 'c')
onkey(lambda: store('shape', rectangle), 'r')
onkey(lambda: store('shape', triangle), 't')
done()
```

# 6. Regla
---

# 7. Link
- [freegames](https://grantjenks.com/docs/freegames/)
- [markdown](https://www.markdownguide.org/cheat-sheet/)

# 8. Images
![mty nl](https://assets.airtrfx.com/media-em/vb/cities/monterrey-MTY.png)

# 9. Tabla
| Syntax | Description |
| ----------- | ----------- |
| TC1001S.101 | Python |
| TC2038.602 | Algoritmos |

# 10. Lista de equipo
- [x] Mariel Perez
- [x] Martha Mendoza
- [ ] Vale Lopez

# 11. emojis
That is so funny! :joy:
😀😆🥹🤣😇🙂
