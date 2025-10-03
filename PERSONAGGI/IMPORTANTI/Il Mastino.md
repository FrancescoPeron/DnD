---
Type: NPC
Stato: In Vita
Gender: Uomo
Age: 28 anni
Location: 
AssociatedGroup: Famiglia Gant
Copper: 40
Silver: 30
Electrum: 0
Gold: 15
Platinum: 0
Armor:
 - Armatura di cuoio borchiato, AC 14
Weapon:
 - Arco lungo, 1d8, a due mani, gittata 45/180 m
 - Spada corta (x2), 1d6, leggera, fine
Items:
 - Kit da esploratore
 - Pozione di Guarigione (x2)
 - Munizioni (20 frecce)
 - Razioni da viaggio (x5)
 - Corda (15 m)
---

## Backstory

"Il Mastino" è un esperto inseguitore al servizio della Famiglia Gant, noto per la sua tenacia e per non mollare mai un obiettivo. Lavora spesso al fianco de "Il Lupo", fornendo supporto a distanza e capacità di tracciamento. Le sue origini sono sconosciute, ma la sua lealtà alla famiglia è incrollabile.

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
name: Il Mastino
layout: Basic 5e Layout Better
size: Media
type: Umanoide
subtype: Umano
alignment: Legale Neutrale
ac: 14 (Armatura di cuoio borchiato)
hp: 34
hit_dice: 4d10+8
speed: 9m
stats:
  - 12
  - 18
  - 14
  - 10
  - 15
  - 8
saves:
  - For: 3
  - Des: 6
  -
  -
skillsaves:
  - Atletica: 3
  - Sopravvivenza: 4
  - Furtività: 6
damage_vulnerabilities: ""
damage_resistances: ""
damage_immunities: ""
condition_immunities: ""
senses: Percezione Passiva 14
languages: Comune
cr: 2
traits:
  - name: Nemico Prescelto
    desc: Ha un nemico prescelto tra Umanoidi (Orchi). Ha vantaggio sulle prove di Saggezza (Sopravvivenza) per seguirne le tracce e prove di Intelligenza per ricavarne informazioni.
  - name: Esploratore Naturale
    desc: Ignora terreni difficili, ha vantaggio sui tiri salvezza contro i pericoli ambientali, e non può essere sorpreso da creature che insegue.
actions:
  - name: Arco Lungo
    desc: "Attacco con Arma a Distanza: +6 al tiro per colpire, gittata 45/180 m, un bersaglio. Colpisce: 8 (1d8 + 4) danni perforanti."
  - name: Spada Corta
    desc: "Attacco con Arma da Mischia: +6 al tiro per colpire, portata 1,5 m, un bersaglio. Colpisce: 7 (1d6 + 4) danni perforanti."
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
```