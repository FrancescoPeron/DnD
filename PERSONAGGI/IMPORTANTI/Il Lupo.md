---
Type: NPC
Stato: In Vita
Gender: Uomo
Age: 25 anni
Location:
AssociatedGroup: Famiglia Gant
Copper: 50
Silver: 20
Electrum: 0
Gold: 10
Platinum: 0
Armor:
- Armatura di maglia (AC 16)
Weapon:
- Spada Lunga, 1d8, versatile (1d10)
- Pugnale, 1d4, leggero, lancio (Gittata 6/18 m)
Items:
- Pozione di Guarigione (x2)
- Razioni da viaggio (x5)
- Scudo
- Zaino
- Coperta
---

## Backstory
Il personaggio, noto come "Il Lupo", è un nobile di rango minore che funge da braccio destro e guardia del corpo per Richard Gant. È stato accolto e cresciuto dalla famiglia Gant fin dall'infanzia, e le sue origini sono sconosciute.

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
name: Il Lupo
layout: Basic 5e Layout Better
size: Media
type: Umanoide
subtype: Tiefling
alignment: Legale Neutrale
ac: 18 
hp: 38
hit_dice: 4d10+12
speed: 9m
stats:
  - 16
  - 12
  - 14
  - 11
  - 12
  - 12
saves:
  - For: 5
  - Cos: 4
  -
  -
skillsaves:
  - Atletica: 5
  - Intuizione: 3
damage_vulnerabilities: ""
damage_resistances: "Fuoco"
damage_immunities: ""
condition_immunities: ""
senses: Percezione Passiva 11
languages: Comune, Infernale
cr: 2
traits:
  - name: Stile di Combattimento (Difesa)
    desc: Finché indossi un'armatura, ottieni un bonus di +1 alla CA.
  - name: Secondo Vento
    desc: Una volta per riposo breve o lungo, puoi usare un'azione bonus per recuperare 1d10 + 4 Punti Ferita.
actions:
  - name: Spada Lunga
    desc: "Attacco con Arma da Mischia: +5 al tiro per colpire, portata 1,5 m, un bersaglio. Colpisce: 8 (1d8 + 3) danni taglienti, o 9 (1d10 + 3) con due mani."
  - name: Pugnale
    desc: "Attacco con Arma da Mischia o a Distanza: +5 al tiro per colpire, portata 1,5 m o gittata 6/18 m, un bersaglio. Colpisce: 5 (1d4 + 3) danni perforanti."
legendary_actions:

reactions:
source: Homebrew
modifier: 0

```