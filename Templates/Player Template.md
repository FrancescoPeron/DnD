---
Type: NPC 
Stato: In Vita
Gender: 
Age: 0 anni
Location: 
AssociatedGroup:  
Copper: 0 
Silver: 0 
Electrum: 0 
Gold: 0
Platinum: 0
Armor:
 - Tipo di Armatura
Weapon:
 - Arma 1, dadi, caratteristiche.
 - Arma 1, dadi, caratteristiche.
Items:
 - oggetto 1
 - oggetto 2
 - oggetto 3
 - oggetto 4
 - oggetto 5
---

## Backstory
Sommario del personaggio


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
name: Mago
layout: Basic 5e Layout Better
size: Media
type: Umanoide
subtype: qualsiasi razza
alignment: Qualsiasi
ac: 12
hp: 22
hit_dice: 5d6+5
speed: 9m
stats:
  - 8
  - 14
  - 12
  - 16
  - 10
  - 10
saves:
  - Int: 5
  - Sag: 2
  -
  -
skillsaves:
  - Arcano: 5
  - Storia: 5
damage_vulnerabilities: ""
damage_resistances: ""
damage_immunities: ""
condition_immunities: ""
senses: Percezione Passiva 10
languages: Comune, Draconico, Elfico
cr: 1
spellnotes: INT (+5), CD 13
spells:
  - name: Dardo di Fuoco
    desc: Trucchetto. Lancia un dardo di fuoco che infligge 1d10 danni da fuoco se colpisce.
  - name: Scudo
    desc: Come reazione, usa uno slot di 1° livello per creare uno scudo che aumenta di 5 la propria CA. Dura per l'attacco.
  - name: Raggio di Gelo
    desc: Trucchetto. Scaglia un raggio di energia fredda che infligge 1d8 danni da freddo e riduce la velocità di 3m.
  - name: Onda Tonante
    desc: Incantesimo di 1° livello. Un'onda di energia sonora infligge 2d8 danni da tuono e spinge i bersagli 3m lontano.
  - name: Passo Velato
    desc: Incantesimo di 2° livello. Ti teletrasporti fino a 9 metri in un punto che puoi vedere.
traits:
  - name: Incantatore
    desc: Il mago è un incantatore di 3° livello. Ha 4 slot incantesimo di 1° livello e 2 di 2° livello.
actions:
  - name: Pugnale
    desc: "Attacco con Arma da Mischia o a Distanza: +4 al tiro per colpire, portata 1,5 m o gittata 6/18 m, un bersaglio. Colpisce: 4 (1d4 + 2) danni perforanti."
legendary_actions:
  - name: 
    desc: ""
  - name: 
    desc: ""
reactions:
  - name: 
    desc: ""
  - name: 
    desc: ""
source: Homebrew
modifier: 0

