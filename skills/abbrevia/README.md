# Abbrevia: uno skill per rivedere testi italiani in stile chiaro e centrato sul lettore

![Linee di testo grigio caotiche cadono in un imbuto arancione e ne escono come rettangoli arancioni ordinati e regolari, trasformando il disordine in testo strutturato](/.github/images/cover.webp)

Ispirato a **[«Пиши, сокращай 2025»](https://sokratil.ru/)** («Scrivi, abbrevia 2025») di Maksim Iljachov e Ljudmila Sarycheva — un classico russo della scrittura professionale che si sposa bene con la tradizione italiana della lingua piana, da Italo Calvino contro l'«antilingua» al lavoro di Tullio De Mauro e Michele Cortelazzo sulla semplificazione del linguaggio amministrativo.

> Questa è la versione italiana. Le versioni per altre lingue sono nel [README principale](../../README.md).

## Cosa fa

Passa a Claude, ChatGPT o Codex un testo professionale in italiano, come un'email, una landing page, un comunicato stampa, un curriculum, una relazione, una presentazione o un'email a freddo. Lo skill lo rivede su cinque livelli:

1. **Pulizia a livello di parola** — toglie riempitivi, vaghezza, vocabolario gonfiato, giudizi vuoti e cliché
2. **Chiarezza a livello di frase** — trasforma nominalizzazioni in verbi, spezza le frasi sovraccariche, mette ordine nei paragrafi
3. **Lotta al burocratese** — sei mosse contro il linguaggio amministrativo e l'aziendalese
4. **Struttura e scopo** — verifica l'azione utile, la definizione del pubblico, la struttura, l'introduzione e la conclusione
5. **Regole di genere** — modelli e controlli per pagine «Chi siamo», curriculum, email a freddo, comunicati stampa, documenti di lavoro, slide e landing page

Lo skill restituisce una versione rivista con il registro delle modifiche e i suggerimenti su cosa aggiungere (fatti, esempi, ricerche).

## Installazione

### Tramite `npx skills` (consigliato)

```bash
npx skills add iamursky/sokrati/tree/main/skills/abbrevia
```

### ChatGPT

1. Scarica l'intera cartella `skills/abbrevia`, compresi `SKILL.md` e `references/`
2. Nella barra laterale di ChatGPT, apri **Plugins → Skills**
3. Seleziona **Create → Upload from your computer** e carica la cartella dello skill
4. Attendi che ChatGPT completi la verifica. Poi seleziona lo skill con `@` o chiedi a ChatGPT di migliorare un testo professionale

### Claude Desktop / Web

1. Scarica l'intera cartella `skills/abbrevia`, compresi [SKILL.md](SKILL.md) e `references/`
2. Vai su **Customize → Skills → + → Upload a skill**
3. Carica la cartella dello skill
4. Lo skill si attiva automaticamente — chiedi a Claude di togliere la fuffa o di rendere il testo «più forte»

### Installazione manuale per Claude Code

```bash
# Personale (disponibile in tutti i progetti)
git clone https://github.com/iamursky/sokrati ~/sokrati
ln -s ~/sokrati/skills/abbrevia ~/.claude/skills/abbrevia

# Per progetto (condiviso con il team via git)
git clone https://github.com/iamursky/sokrati .sokrati
ln -s .sokrati/skills/abbrevia .claude/skills/abbrevia
```

## Come usarlo

Lo skill si attiva automaticamente quando:

- Chiedi a Claude, ChatGPT o Codex di rivedere, controllare, ripulire o migliorare un testo professionale in italiano
- Menzioni «stile informativo», «infostyle», «Iljachov» (o «Ilyahov»), «Glavred», «parole vuote», «burocratese», «linguaggio amministrativo», «antilingua» o «aziendalese»
- Chiedi di togliere la «fuffa» dal testo, di renderlo «più forte», «più asciutto» o «più diretto»
- Chiedi di riscrivere qualcosa in «lingua semplice», «italiano chiaro» o «lingua umana»

### Esempi

**Riscrittura completa:**

> Riscrivi questo testo per la landing page in stile chiaro: [testo]

**Revisione senza riscrittura:**

> Dammi un feedback su questa email. Cosa si può migliorare? [testo]

**Domanda sulle tecniche:**

> Come si scrive una pagina «Chi siamo» in stile informativo?

## Crediti

Lo skill è ispirato al libro **«Пиши, сокращай 2025»** di Maksim Iljachov e Ljudmila Sarycheva. Non è un prodotto ufficiale degli autori del libro e non riproduce il testo originale. Le idee e le tecniche appartengono agli autori; questo skill le interpreta come un flusso di lavoro per un assistente IA. Se leggi il russo e il libro ti piace, sostieni gli autori comprandolo al link qui sopra.
