# Escurça — un skill de Claude per editar textos professionals en català, en estil planer i centrat en el lector

![Línies de text grises i caòtiques cauen dins d'un embut taronja i en surten convertides en rectangles taronges nets i ordenats: del desordre al text estructurat](/.github/images/cover.webp)

Inspirat en **[«Пиши, сокращай 2025»](https://sokratil.ru/)** («Escriu, escurça 2025») de Maxim Ilyahov i Liudmila Sarítxeva.

> Aquesta és la versió catalana. Les versions per a altres llengües són al [README de l'arrel](../../README.md).

## Què fa

Passa-li a Claude qualsevol text professional en català —un correu, una landing page, una pàgina «Qui som», una nota de premsa, un currículum, una carta de presentació, un informe, una presentació o un missatge en fred— i l'editarà en cinc nivells:

1. **Neteja a nivell de paraula** — suprimeix marcadors buits, imprecisions, vocabulari inflat, judicis sense proves i tòpics
2. **Claredat a nivell de frase** — converteix les nominalitzacions en verbs, parteix les frases sobrecarregades i posa ordre als paràgrafs
3. **Lluita contra el llenguatge burocràtic** — aplica sis tàctiques (primer el contingut, títol útil, cura activa, fora la passiva reflexa, etc.)
4. **Estructura i propòsit** — comprova l'acció útil, l'audiència, l'estructura, la introducció i la conclusió
5. **Regles de gènere** — plantilles i comprovacions per a pàgines «Qui som», currículums, missatges en fred, notes de premsa, documents de feina, presentacions i landing pages

A més, vigila fenòmens propis del català: cadenes de pronoms febles, passiva reflexa abusada, castellanismes («bueno», «vale», «entonces»), diminutius cursis, «el fet de + infinitiu» i cadenes de relatius compostos.

L'skill torna una versió editada amb la llista de canvis i recomanacions del que l'autor hauria d'afegir (fets, exemples, recerca).

## Instal·lació

### Via `npx skills` (recomanat)

```bash
npx skills add iamursky/sokrati/tree/main/skills/escurca
```

### Claude Desktop / Web

1. Descarrega [SKILL.md](SKILL.md)
2. Vés a **Customize → Skills → + → Upload a skill**
3. Carrega el fitxer `SKILL.md`
4. L'skill s'activarà automàticament —demana a Claude que tregui la palla d'un text o que el faci «més fort»

### Instal·lació manual per a Claude Code

```bash
# Personal (disponible a tots els projectes)
git clone https://github.com/iamursky/sokrati ~/sokrati
ln -s ~/sokrati/skills/escurca ~/.claude/skills/escurca

# Per projecte (compartit amb l'equip per git)
git clone https://github.com/iamursky/sokrati .sokrati
ln -s .sokrati/skills/escurca .claude/skills/escurca
```

## Com s'utilitza

L'skill s'activa automàticament quan:

- Demanes a Claude editar, revisar, netejar o millorar qualsevol text professional en català
- Esmentes «estil informatiu», «infostyle», «Ilyahov», «Glavred», «paraules buides», «paraules mosca» o «llenguatge burocràtic»
- Demanes treure la palla d'un text o fer-lo «més fort»
- Demanes reescriure alguna cosa en «llenguatge planer» o «català planer»

### Exemples

**Edició completa:**

> Edita el text d'aquesta landing en estil informatiu: [text]

**Revisió sense reescriure:**

> Dona'm crítica d'aquest correu. Què es pot millorar? [text]

**Pregunta sobre la tècnica:**

> Com s'ha d'escriure un «Qui som» en estil informatiu?

## Autoria

L'skill s'inspira en el llibre **«Пиши, сокращай 2025»** de Maxim Ilyahov i Liudmila Sarítxeva. No és un producte oficial dels autors del llibre ni reprodueix el text original. Les idees i tècniques pertanyen als autors; aquest skill és una interpretació d'aquestes idees en forma d'algorismes per a Claude. Si llegeixes rus i t'agrada el llibre, dona suport als autors comprant-lo a l'enllaç de més amunt.
