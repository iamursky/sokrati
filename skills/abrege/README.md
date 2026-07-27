# Abrège: un skill pour éditer le français professionnel en style clair, centré sur le lecteur

![Des lignes de texte grises et désordonnées tombent dans un entonnoir orange et en ressortent en rectangles oranges nets et alignés, transformant le désordre en texte structuré](/.github/images/cover.webp)

Inspiré par **[«Пиши, сокращай 2025»](https://sokratil.ru/)** («Écris, abrège 2025») de Maxime Iliakhov et Lioudmila Saritcheva.

> Ceci est la version française. Pour les autres langues, voir le [README à la racine](../../README.md).

## Ce que ça fait

Donnez à Claude, ChatGPT ou Codex un texte professionnel en français, par exemple un courriel, une page d'accueil, un communiqué de presse, un CV, un rapport, une présentation ou un courriel de prospection. Le skill l'édite sur cinq niveaux :

1. **Nettoyage au niveau des mots** — coupe les formules de remplissage, le vague, le vocabulaire ampoulé, les jugements vides, les clichés et les anglicismes inutiles
2. **Clarté au niveau des phrases** — transforme les nominalisations en verbes, casse les phrases interminables, remet de la discipline dans les paragraphes
3. **Combat contre la langue de bois et le jargon administratif** — sept manœuvres pour démonter les formules creuses, les chaînes de «de», les tournures impersonnelles et le sabir corporate
4. **Structure et finalité** — vérifie l'action utile, l'audience, la structure, l'introduction et la conclusion
5. **Règles de genre** — modèles et contrôles pour les pages «À propos», CV, lettres de motivation, courriels à froid, communiqués de presse, documents de travail, diapositives, pages d'accueil

Le skill renvoie une version éditée avec un journal des changements et des recommandations sur ce que l'auteur devrait ajouter (faits, exemples, recherche).

## Installation

### Via `npx skills` (recommandé)

```bash
npx skills add iamursky/sokrati/tree/main/skills/abrege
```

### ChatGPT

1. Téléchargez le dossier `skills/abrege` complet, avec `SKILL.md` et `references/`
2. Dans la barre latérale de ChatGPT, ouvrez **Plugins → Skills**
3. Sélectionnez **Create → Upload from your computer**, puis téléversez le dossier du skill
4. Attendez la fin de l'analyse par ChatGPT. Sélectionnez ensuite le skill avec `@` ou demandez à ChatGPT d'améliorer un texte professionnel

### Claude Desktop / Web

1. Téléchargez le dossier `skills/abrege` complet, avec [SKILL.md](SKILL.md) et `references/`
2. Allez dans **Customize → Skills → + → Upload a skill**
3. Téléversez le dossier du skill
4. Le skill se déclenche automatiquement — demandez à Claude de couper le gras, de virer la langue de bois ou de rendre un texte «plus fort»

### Installation manuelle pour Claude Code

```bash
# Personnel (disponible dans tous les projets)
git clone https://github.com/iamursky/sokrati ~/sokrati
ln -s ~/sokrati/skills/abrege ~/.claude/skills/abrege

# Par projet (partagé avec l'équipe via git)
git clone https://github.com/iamursky/sokrati .sokrati
ln -s .sokrati/skills/abrege .claude/skills/abrege
```

## Comment l'utiliser

Le skill se déclenche automatiquement quand vous :

- Demandez à Claude, ChatGPT ou Codex de relire, corriger, alléger ou améliorer n'importe quel texte professionnel en français
- Mentionnez «style informatif», «infostyle», «Iliakhov», «Glavred», «mots de remplissage», «langue de bois», «jargon administratif» ou «anglicismes inutiles»
- Demandez à l'assistant de «couper le gras», «virer le bla-bla», «virer la langue de bois», ou d'écrire en «français normal»

### Exemples

**Refonte complète :**

> Édite-moi cette page d'accueil en style informatif : [texte]

**Relecture sans réécriture :**

> Donne-moi un retour sur ce courriel. Qu'est-ce qui peut être amélioré ? [texte]

**Question sur les procédés :**

> Comment rédiger une rubrique «À propos» en style informatif ?

## Paternité

Le skill s'inspire de **«Пиши, сокращай 2025»** de Maxime Iliakhov et Lioudmila Saritcheva. Ce n'est pas un produit officiel des auteurs et il ne reproduit pas le texte original. Les idées et procédés appartiennent aux auteurs ; ce skill les interprète comme un flux de travail pour un assistant IA. Si vous lisez le russe et que le livre vous plaît, soutenez les auteurs en l'achetant via le lien ci-dessus.
