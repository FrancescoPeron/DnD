---
Type: NPC
Stato: In vita
Gender: Femmina
Age: 24 anni
Location: Underhall
AssociatedGroup: Famiglia Gant,
Copper: 0
Silver: 0
Electrum: 0
Gold: 0
Platinum: 0
Armor:
  - Armatura di cuoio borchiato
Weapon:
  - Pugnale Magico, 1d4 + 3 danni perforanti, magico
Items:
  - Pozione di cura minore (x2)
  - Liuto
---

## Backstory
Figlia di [[Xenophilious Gant]], ha sedotto con un incantesimo di charme su persone il figlio del conte limitrofo. Ciò è stato progettato per avere il supporto del conte quando la famiglia Gant salirà al potere, oltre che avere un esercito e  un castello pronto ad ospitarli in caso di pericolo. 
Il figlio del conte [[Onyx Oberon]] in realtà era già innamorato di Isabelle, per cui anche se distrutto l'incantesimo continuerà a stare dalla parte di Isabelle. 
Ella gestisce l'andamento delle proprietà della famiglia.

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
name: Isabelle Gant
layout: Basic 5e Layout Better
size: Media
type: Umanoide
subtype: umano
alignment: Malvagio, Neutrale
ac: 14
hp: 35
hit_dice: 5d8+5
speed: 9m
stats:
  - 8
  - 14
  - 12
  - 10
  - 10
  - 16
saves:
  - Dex: 5
  - Cha: 6
skillsaves:
  - Persuasione: 6
  - Inganno: 6
  - Performance: 6
damage_vulnerabilities: ""
damage_resistances: ""
damage_immunities: ""
condition_immunities: ""
senses: Percezione Passiva 10
languages: Comune, Nanico
cr: 3
spellnotes: CHA (+6), CD 14
spells:
  - name: Ispirazione Bardica (Azione Bonus)
    desc: Come azione bonus, puoi scegliere una creatura a portata che ti può sentire, per darle un dado di ispirazione bardica (1d8). Una volta per la prossima ora, la creatura può sommare il risultato a un tiro per colpire, un tiro salvezza o un'abilità.
  - name: Illusione Minore (Trucchetto)
    desc: Crei il suono o l'immagine di un oggetto inanimato a portata. L'illusione può occupare uno spazio di 1,5 metri cubi.
  - name: Charme su persone (1° Livello)
    desc: Incanta un umanoide che diventa amichevole nei tuoi confronti per 1 ora.
  - name: Passo velato (2° Livello)
    desc: Ti teletrasporti fino a 9 metri in uno spazio che puoi vedere.
  - name: Paura (3° Livello)
    desc: Fai sì che un gruppo di creature diventi spaventato dalla paura per la durata dell'incantesimo.
traits:
  - name: Incantatore
    desc: "Il bardo è un incantatore di 5° livello. Dispone di 4 slot incantesimo di 1° livello, 3 di 2° livello e 2 di 3° livello. Isabelle ha anche 3 usi di Ispirazione Bardica per riposo lungo, con un dado di 1d8."
actions:
  - name: Pugnale Magico
    desc: "Attacco con Arma da Mischia o a Distanza Magica: +6 al tiro per colpire, portata 1,5 m o gittata 6/18 m, un bersaglio. Colpisce: 5 (1d4 + 3) danni perforanti. Questo è un attacco magico."
legendary_actions:
  - name: Sifone Sanguigno (1 azione)
    desc: "Isabelle infligge 2d4 danni necrotici a una creatura nel raggio di 9m che ha una ferita aperta. Isabelle recupera un numero di punti ferita pari al danno inflitto."
reactions:
source: Homebrew
modifier: 0

```
