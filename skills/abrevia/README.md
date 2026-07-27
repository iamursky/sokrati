# Abrevia: una habilidad para editar textos profesionales en español con un estilo claro y centrado en el lector

![Líneas grises y caóticas de texto caen en un embudo naranja y salen como rectángulos naranjas ordenados y uniformes, transformando el desorden en un texto estructurado](/.github/images/cover.webp)

Inspirada en **[«Пиши, сокращай 2025»](https://sokratil.ru/)** («Escribe, abrevia 2025») de Maxim Iliajov y Liudmila Sárycheva, un clásico ruso sobre escritura profesional que dialoga con la tradición hispánica del lenguaje claro y la lucha contra el lenguaje administrativo.

> Esta es la versión en español. Las versiones en otras lenguas están en el [README de la raíz](../../README.md).

## Qué hace

Pásale a Claude, ChatGPT o Codex un texto profesional en español, como un correo, una página de aterrizaje, una nota de prensa, un currículum, un informe, una presentación o un correo en frío. La habilidad lo edita en cinco niveles:

1. **Limpieza al nivel de las palabras** — quita muletillas, imprecisiones, vocabulario inflado, valoraciones vacías y clichés
2. **Claridad al nivel de la oración** — convierte sustantivos derivados de verbos en verbos, rompe oraciones sobrecargadas, deshace las cadenas de «de», aprieta la disciplina del párrafo
3. **Lucha contra el lenguaje administrativo** — seis movimientos contra el lenguaje cancilleresco que se cuela en la prosa corporativa y oficial
4. **Estructura y propósito** — revisa la acción útil, el público, la estructura, la entradilla y el cierre
5. **Reglas por género** — plantillas y comprobaciones para páginas «Quiénes somos», currículums, cartas de presentación, correos en frío, notas de prensa, documentos internos, presentaciones y páginas de aterrizaje

La habilidad devuelve una versión editada con una lista de cambios y recomendaciones sobre qué debería añadir el autor (hechos, ejemplos, investigación).

## Instalación

### Vía `npx skills` (recomendado)

```bash
npx skills add iamursky/sokrati/tree/main/skills/abrevia
```

### ChatGPT

1. Descarga la carpeta `skills/abrevia` completa, incluidos `SKILL.md` y `references/`
2. En la barra lateral de ChatGPT, abre **Plugins → Skills**
3. Selecciona **Create → Upload from your computer** y sube la carpeta de la habilidad
4. Espera a que ChatGPT termine de revisar la habilidad. Después, selecciónala con `@` o pide a ChatGPT que mejore un texto profesional

### Claude Desktop / Web

1. Descarga la carpeta `skills/abrevia` completa, incluidos [SKILL.md](SKILL.md) y `references/`
2. Ve a **Customize → Skills → + → Upload a skill**
3. Sube la carpeta de la habilidad
4. La habilidad se activa automáticamente: pide a Claude que quite la «paja» de un texto o que lo deje «más claro»

### Instalación manual para Claude Code

```bash
# Personal (disponible en todos los proyectos)
git clone https://github.com/iamursky/sokrati ~/sokrati
ln -s ~/sokrati/skills/abrevia ~/.claude/skills/abrevia

# Para un proyecto concreto (compartido con el equipo por git)
git clone https://github.com/iamursky/sokrati .sokrati
ln -s .sokrati/skills/abrevia .claude/skills/abrevia
```

## Cómo usarla

La habilidad se activa automáticamente cuando:

- Pides editar, revisar o mejorar cualquier texto profesional en español
- Mencionas «estilo informativo», «infoestilo», «Iliajov», «Glavred», «palabras de relleno», «muletillas», «lenguaje administrativo», «lenguaje burocrático» o «lenguaje cancilleresco»
- Pides quitar la «paja» o la «hojarasca» de un texto, eliminar clichés o dejarlo «más fuerte»
- Pides reescribir algo en «lenguaje llano», «lenguaje claro» o «lenguaje sencillo»

### Ejemplos

**Edición completa:**

> Edita este texto de la landing en estilo claro: [texto]

**Revisión sin reescribir:**

> Dame retroalimentación sobre este correo. ¿Qué se puede mejorar? [texto]

**Pregunta sobre una técnica:**

> ¿Cómo escribo el apartado «Quiénes somos» en lenguaje claro?

## Autoría

Esta habilidad se inspira en **«Пиши, сокращай 2025»** de Maxim Iliajov y Liudmila Sárycheva. No es un producto oficial de los autores del libro y no reproduce el texto original. Las ideas y técnicas son de los autores; esta habilidad las interpreta como un flujo de trabajo para un asistente de IA. Si lees ruso y te gusta el libro, apoya a los autores comprándolo en el enlace de arriba.
