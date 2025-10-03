---
Type: NPC
Stato: In Vita
Gender: Maschio
Age: "32"
Location: Gran Burrone
AssociatedGroup: Famiglia Gant
Copper: 0
Silver: 0
Electrum: 0
Gold: 0
Platinum: 0
Armor:
  - Armatura a piastre
Weapon:
  - Spadone della Vendetta Caduta, 2d6+3 danni + 1d4 danni necrotici
  - Picca del Giuramento Spezzato
Items:
  - Nessuno
---

## Backstory
Figlio primogenito di [[Xenophilious Gant]], gli è stato inculcato fin da bambino il mantra di fare tutto per la famiglia. Bravo con la spada, è entrato nell'esercito ed è stato lui a riportare in auge il nome Gant. All'età di 33 anni è diventato capo delle guardie della capitale della contea, permettendogli di creare una piccola milizia dentro la regione del conte.
Il suo obiettivo è di usare le creature schiavizzate da [[Richard Gant]] per spaventare la popolazione e per poi salvarla, aumentando così la sua presa sulla contea.

L'intelligenza non è il suo forte, ma è un condottiero amato dai cittadini.


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
name: Lucius Gant
layout: Basic 5e Layout Better
size: Media
type: Umanoide
subtype: qualsiasi razza
alignment: Malvagio
ac: 18
hp: 60
hit_dice: 6d10+24
speed: 9m
stats:
  - 16
  - 10
  - 14
  - 8
  - 12
  - 14
saves:
  - Str: 6
  - Con: 5
  - Sag: 4
  - Car: 5
skillsaves:
  - Atletica: 6
  - Intimidire: 5
damage_vulnerabilities: ""
damage_resistances: ""
damage_immunities: ""
condition_immunities: ""
senses: Percezione Passiva 11
languages: Comune
cr: 4
spellnotes: CAR (+2), CD 13
spells:
  - name: Incantesimi (1° livello)
    desc: |-
        - **Castigo Infernale**: Quando un nemico a portata colpisce Lucius, può usare la sua reazione e uno slot incantesimo per costringere il nemico a superare un tiro salvezza o subire 2d10 danni da fuoco.
        - **Scudo Divino**: Come reazione, usa uno slot di 1° livello per aumentare la CA di 5. Dura fino al tuo prossimo turno.
  - name: Incantesimi (2° livello)
    desc: |-
        - **Passo Velato**: Ti teletrasporti fino a 9 metri in un punto che puoi vedere.
        - **Arma Magica**: Tocchi un'arma non magica e la rendi magica per 1 ora.
traits:
  - name: Giuramento Abbandonato
    desc: Lucius ha rinunciato al suo giuramento, ottenendo poteri che derivano dalla sua dedizione al potere e alla sua famiglia.
  - name: Incantatore
    desc: "Il paladino è un incantatore di 6° livello. Ha 4 slot incantesimo di 1° livello e 2 di 2° livello."
  - name: Aura di Protezione
    desc: "Finche è cosciente, Lucius e le creature amiche a 3 metri da lui ottengono un bonus ai tiri salvezza pari al suo modificatore di Carisma (+2)."
  - name: Picca del Giuramento Spezzato
    desc: "Questa picca magica ritorna automaticamente nella mano di Lucius dopo essere stata lanciata. Infligge 1d6 danni perforanti e ha un raggio di lancio di 6/18m."
actions:
  - name: Spadone della Vendetta Caduta
    desc: "Attacco con Arma da Mischia: +6 al tiro per colpire, portata 1,5 m, un bersaglio. Colpisce: 10 (2d6 + 3) danni taglienti, più 2 (1d4) danni necrotici aggiuntivi. Questo attacco è magico."
  - name: Colpo Divino
    desc: "Quando Lucius colpisce con un'arma da mischia, può usare uno slot incantesimo per infliggere danni radianti aggiuntivi al bersaglio (2d8 per slot di 1° livello, 3d8 per slot di 2° livello)."
legendary_actions:
  - name: Giuramento Abbandonato (1 azione leggendaria)
    desc: "Quando Lucius raggiunge 0 punti ferita, può usare la sua volontà per attivare un'azione leggendaria. Lucius recupera un numero di punti ferita pari a 2d8 + il suo modificatore di Carisma (+2) ed entra in uno stato di ira. Per 1 minuto, ottiene resistenza ai danni contundenti, perforanti e taglienti. I suoi attacchi con lo spadone infliggono 2 danni aggiuntivi. Questa azione può essere usata solo una volta per incontro."
reactions:

source: Homebrew
modifier: 0

```
