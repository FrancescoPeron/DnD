---
Type: NPC
Level: 4
Race: Mezzelfo
Stato: In Vita
Alignment: Neutrale
Gender: Maschio
Age: "25"
Location: Emberdawn
Class: Ladro
Subclass: NONE
AssociatedGroup: NONE
Copper: 0
Silver: 0
Electrum: 0
Gold: 150
Platinum: 0
Armor:
  - Armatura di cuoio
Weapon:
  - Pugnali avvelenati
  - Arco Lungo
Items:
  - Pozione di cura minore
  - Frecce elementali (x10)
  - Frecce (x20)
---

## Backstory
Figlio bastardo di Lucius Gant e di una donna rapita dalla famiglia Gant. È disposto a molto per il suo fine, e cercherà di uccidere la famiglia del BBEG per vendetta sulla sua vita, ma non vuole cercare la madre.

Quando il ragazzo aveva pochi anni, la madre è riuscita a scappare con il figlio prima che fosse sacrificato al ramo legittimo, ma lo ha abbandonato da una famiglia nella città di [[Emberdawn]], che ha cresciuto il ragazzo. Passati un paio d'anni, il ragazzo è stato braccato da un gruppo di spie che lo aveva riconosciuto, costringendo il ragazzo a darsi alla macchia.
Così ha avuto modo di costruire una gilda di ladri al fine di scoprire chi gli ha mandato i sicari.
Al momento in cui il party arriva da lui, ha scoperto il nome della famiglia mandante dei sicari, la famiglia Gant, ma non sa il perché.
La gilda gli ha permesso di scoprire subito appena avvenuto che la bussola è stata presa da un gruppo di avventurieri e che si stanno dirigendo da lui.


## Inventario
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
name: Alvas
image: [[elf_rogue.webp]]
layout: Basic 5e Layout Better
size: Media
type: Umanoide
subtype: mezzelfo
alignment: Neutrale
ac: 16
hp: 26
hit_dice: 4d8+4
speed: 9m
stats:
  - 10
  - 16
  - 12
  - 14
  - 10
  - 10
saves:
  - Dex: 5
  - Int: 4
skillsaves:
  - Acrobazia: 5
  - Indagare: 4
  - Furtività: 7
damage_vulnerabilities: ""
damage_resistances: ""
damage_immunities: ""
condition_immunities: ""
senses: Percezione Passiva 10
languages: Comune, Elfico
cr: 2
spellnotes: ""
spells:
  - name:
    desc: ""
traits:
  - name: Azione Scaltra
    desc: "Alvas può usare la sua azione bonus per fare un'azione di Scattare, Disimpegnarsi o Nascondersi."
  - name: Attacco Furtivo
    desc: "Una volta per turno, Alvas può infliggere 2d6 danni aggiuntivi a un bersaglio che colpisce con un attacco con un'arma da finesse o a distanza, se ha vantaggio al tiro per colpire."
  - name: Volontà Ladresca
    desc: "Alvas ha la capacità di eseguire una seconda azione bonus ogni turno. Questa azione extra può essere usata solo per fare una delle opzioni disponibili con l'Azione Scaltra."
  - name: Lame Avvelenate
    desc: "I pugnali di Alvas sono costantemente ricoperti di un veleno magico. Qualsiasi creatura colpita da un suo pugnale deve superare un tiro salvezza sulla Costituzione con CD 12 o subire 1d4 danni da veleno aggiuntivi e diventare avvelenata per 1 minuto. Il bersaglio può ripetere il tiro salvezza alla fine di ogni suo turno."
actions:
  - name: Pugnale Avvelenato
    desc: "Attacco con Arma da Mischia: +5 al tiro per colpire, portata 1,5 m, un bersaglio. Colpisce: 6 (1d4 + 3) danni perforanti. Se il bersaglio fallisce il tiro salvezza, subisce 1d4 danni da veleno aggiuntivi e viene avvelenato per 1 minuto."
  - name: Arco Lungo
    desc: "Attacco con Arma a Distanza: +5 al tiro per colpire, gittata 45/180 m, un bersaglio. Colpisce: 7 (1d8 + 3) danni perforanti. Può usare le frecce elementali per cambiare il tipo di danno."
legendary_actions:
  - name: Colpo Sanguinario (1 azione leggendaria)
    desc: "Alvas effettua un attacco a distanza contro una creatura nel raggio di 4.5m. Se colpisce, l'attacco infligge 2d4 danni necrotici aggiuntivi. Alvas recupera un numero di punti ferita pari al danno necrotico inflitto. Questa azione può essere usata due volte per riposo lungo."
reactions:
  - name:
    desc: ""
source: Homebrew
modifier: 0
```