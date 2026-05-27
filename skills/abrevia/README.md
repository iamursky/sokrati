# Abrevia — una habilidad de Claude para editar textos profesionales en español con un estilo claro y centrado en el lector

![Líneas grises y caóticas de texto caen en un embudo naranja y salen como rectángulos naranjas ordenados y uniformes, transformando el desorden en un texto estructurado](/.github/images/cover.webp)

Inspirada en **[«Пиши, сокращай 2025»](https://sokratil.ru/)** («Escribe, abrevia 2025») de Maxim Iliajov y Liudmila Sárycheva, un clásico ruso sobre escritura profesional que dialoga con la tradición hispánica del lenguaje claro y la lucha contra el lenguaje administrativo.

> Esta es la versión en español. Las versiones en otras lenguas están en el [README de la raíz](../../README.md).

## Qué hace

Pásale a Claude cualquier texto profesional en español — un correo, una página de aterrizaje, una página «Quiénes somos», una nota de prensa, un currículum, una carta de presentación, un informe, una presentación o un correo en frío — y lo edita en cinco niveles:

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

### Claude Desktop / Web

1. Descarga [SKILL.md](SKILL.md)
2. Ve a **Customize → Skills → + → Upload a skill**
3. Sube `SKILL.md`
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

Esta habilidad se inspira en **«Пиши, сокращай 2025»** de Maxim Iliajov y Liudmila Sárycheva. No es un producto oficial de los autores del libro y no reproduce el texto original. Las ideas y técnicas son de los autores; esta habilidad es una interpretación de esas ideas convertida en algoritmos para Claude. Si lees ruso y te gusta el libro, apoya a los autores comprándolo en el enlace de arriba.
