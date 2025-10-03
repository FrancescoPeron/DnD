---
 Type: NPC 
 Stato: In Vita 
 Gender: Femmina 
 Age: 120 anni 
 Location: Emberdawn 
 AssociatedGroup: Nessuno (Attualmente un'agente solitaria) 
 Copper: 0 
 Silver: 0 
 Electrum: 0 
 Gold: 75 
 Platinum: 0
 Armor:
 - Armatura in Cuoio Borchiato (AC 12 + DEX mod)
 Weapon:
 - Spada Corta  1d6 + 3 danno perforante, Finesse, Leggera.
 - Pugnale  1d4 + 3 danno perforante, Finesse, Leggera, Lanciabile (Gittata 6/18m).
 Items:
 - Borsa da Scasso
 - Tre pugnali da lancio extra
 - Mantello scuro con cappuccio
 - Fiala di veleno base (per 1 arma)
 - Una piccola borsa con 50 piedi di corda sottile
 - Una gemma di sangue, apparentemente senza valore, ma che per Lyra ha un significato particolare
---
## Backstory

Lyra è una Drow di 120 anni, un'agente solitaria e un'assassina esperta che opera principalmente nell'ombra di [[Emberdawn]]. Il suo passato è costellato di tradimenti e vendette, che l'hanno resa sospettosa e guardinga nei confronti di chiunque. Nonostante la sua natura calcolatrice, a volte la sua fredda logica può essere interrotta da improvvise esplosioni di furia, retaggio della sua indole caotica e del suo allineamento malvagio.

Disprezza la luce solare diretta e ogni forma di autorità, preferendo muoversi indisturbata tra le ombre. I traditori sono i suoi nemici più acerrimi, e il rumore eccessivo e le persone troppo fiduciose la irritano profondamente. Estremamente attenta ai dettagli e un'osservatrice acuta, Lyra possiede una memoria eccezionale per i volti e le informazioni, rendendola una spia e un'assassina formidabile. È rapida nel formulare piani e adatta a ogni nuova situazione, ma la sua natura introversa e distante la porta a evitare il contatto visivo prolungato, parlando solo quando strettamente necessario. Quando costretta a interagire, è acuta e perspicace, abilissima nel manipolare le situazioni a suo vantaggio per ottenere oro o informazioni preziose. La piccola gemma di sangue che porta con sé, apparentemente senza valore, racchiude per Lyra un significato particolare, forse legato a un giuramento o a un ricordo doloroso.

```dataviewjs

dv.header(3, "Equipaggiamento:");

dv.header(4, "Armatura:");
let armorItems = dv.current().Armor; 
if (armorItems) { 
    if (!Array.isArray(armorItems)) {
        armorItems = [armorItems]; 
    }
    armorItems.forEach(item => {
        dv.el("li", item); 
    });
} else {
    dv.paragraph("Nessun equipaggiamento specificato.");
}

dv.header(4, "Armi:");
let wepItems = dv.current().Weapon; 
if (wepItems) { 
    if (!Array.isArray(wepItems)) {
        wepItems = [wepItems]; 
    }
    wepItems.forEach(item => {
        dv.el("li", item); 
    });
} else {
    dv.paragraph("Nessun equipaggiamento specificato.");
}

dv.header(4, "Item:");
let Items = dv.current().Items; 
if (Items) { 
    if (!Array.isArray(Items)) {
        Items = [Items]; 
    }
    Items.forEach(item => {
        dv.el("li", item); 
    });
} else {
    dv.paragraph("Nessun equipaggiamento specificato.");
}
```

## Scheda Personaggio
```statblock
name: Lyra
image: [[female_darkelf_rogue.webp]]
layout: Basic 5e Layout Better
size: Media
type: Umanoide
subtype: Drow
alignment: Caotico Malvagio
ac: 15
hp: 22
hit_dice: 3d8
speed: 9m
stats: [10, 16, 14, 12, 10, 8]
saves:
- Destrezza: 5
- Costituzione: 4
- Saggezza: 2
- Carisma: 1
skillsaves:
- Furtività: 7
- Percezione: 2
- Indagare: 3
- Acrobazia: 5
- Inganno: 1
damage_vulnerabilities: ""
damage_resistances: "Veleno"
damage_immunities: ""
condition_immunities: ""
senses: Percezione Passiva 12, Scurovisione 36m
languages: Comune, Sottocomune, Drow
cr: 2
spellnotes: INT (+31), CD 12
traits:
  - name: Resistenze Drow
    desc: "Lyra ha vantaggio sui tiri salvezza contro gli incantesimi e altre effetti magici."
  - name: Addestramento da Assassino
    desc: "Resistenza al danno da veleno."
  - name: Furtività Drow
    desc: "Lyra è esperta nel muoversi nell'ombra, rendendola difficile da individuare."
actions:
  - name: Attacco con Spada Corta
    desc: "Attacco con arma da mischia: +5 al tiro per colpire, portata 1.5m, un bersaglio. Colpito: 1d6 + 3 danni perforanti."
  - name: Attacco con Pugnale
    desc: "Attacco con arma da mischia o a distanza: +5 al tiro per colpire, portata 1.5m o gittata 6/18m, un bersaglio. Colpito: 1d4 + 3 danni perforanti."
  - name: Attacco Furtivo (1/turno)
    desc: "Una volta per turno, se Lyra ha vantaggio al tiro per colpire contro una creatura, o se un'altra nemesi del bersaglio si trova entro 1.5 metri dal bersaglio e non è inabile, Lyra può infliggere 2d6 danni aggiuntivi al bersaglio se lo colpisce con un attacco con arma Finesse o a Distanza. Non ha bisogno di vantaggio al tiro per colpire se l'attacco proviene da una posizione nascosta."
spells:
  - name: Luce Danzante
    desc: "Puoi creare fino a quattro luci a tua scelta entro 36 metri che possono assumere l'aspetto di torce, lanterne, sfere luminose o forme vagamente umanoidi. Puoi farle fluttuare ed emettere luce fioca. Puoi usare questo incantesimo a volontà, senza spendere slot incantesimo."
  - name: Tenebre
    desc: "Puoi creare una sfera di tenebra magica di 4,5 metri di raggio su un punto che puoi vedere entro 18 metri. La tenebra si propaga dietro gli angoli. Una creatura con scurovisione non può vedere attraverso questa tenebra, e la luce normale o magica non può illuminarla. Puoi usare questo incantesimo una volta per ogni riposo lungo."
  - name: Bagliore Fatato
    desc: "Come azione, puoi far brillare di luce fatata fino a due creature a tua scelta entro 18 metri. Ogni bersaglio è illuminato e non beneficia della condizione nascosto, e gli attacchi contro di esso hanno vantaggio. Puoi usare questo incantesimo una volta per ogni riposo lungo."
legendary_actions: ""
reactions: ""


```



