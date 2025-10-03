---
Type: NPC
Stato: In Vita
Gender: Maschio
Age: "22"
Location: Pietra di Shor
AssociatedGroup: [[Congrega dell'Ombra]]
Copper: 0
Silver: 0
Electrum: 0
Gold: 0
Platinum: 0
Armor:
 - Nessuna
Weapon:
 - Bastone, 1d6-1, versatile (1d8)
Items:
 - Pergamene di Evoca Elementale (x2)
 - Sfera del Comando Elementale
---

## Backstory
Terzo figlio di [[Xenophilious Gant]]. È un mago che vuole spingere al limite le potenzialità della magia sull'uomo. Possiede un laboratorio in cui procede con gli esperimenti cominciati dal padre tempo addietro. L'obiettivo è di creare un oggetto che permetta di controllare le entità con intelligenza inferiore per dominarle e usarle come schiavi. Usa la sua organizzazione, la [[Congrega dell'Ombra]], per trovare nuove cavie e/o nuovi scagnozzi per fare il lavoro sporco. Vive a [[Pietra di Shor]], dove è conosciuto per essere uno scapolo d'oro e un intenditore di oggetti magici.


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
name: Richard Gant
layout: Basic 5e Layout Better
size: Media
type: Umanoide
subtype: umano
alignment: neutrale malvagio
ac: 12
hp: 28
hit_dice: 6d6+6
speed: 9m
stats:
  - 8
  - 14
  - 12
  - 16
  - 10
  - 10
saves:
  - Int: 6
  - Sag: 3
skillsaves:
  - Arcano: 6
  - Storia: 6
damage_vulnerabilities: ""
damage_resistances: ""
damage_immunities: ""
condition_immunities: ""
senses: Percezione Passiva 10
languages: Comune, Draconico, Elfico
cr: 4
spellnotes: INT (+3), CD 14
spells:
  - name: Dardo di Fuoco (Trucchetto)
    desc: Lancia un dardo di fuoco che infligge 1d10 danni da fuoco se colpisce.
  - name: Raggio di Gelo (Trucchetto)
    desc: Scaglia un raggio di energia fredda che infligge 1d8 danni da freddo e riduce la velocità di 3m.
  - name: Scudo (1° livello)
    desc: Come reazione, usa uno slot di 1° livello per creare uno scudo che aumenta di 5 la propria CA. Dura per l'attacco.
  - name: Onda Tonante (1° livello)
    desc: Un'onda di energia sonora infligge 2d8 danni da tuono e spinge i bersagli 3m lontano.
  - name: Passo Velato (2° livello)
    desc: Ti teletrasporti fino a 9 metri in un punto che puoi vedere.
  - name: Palla di Fuoco (3° livello)
    desc: Un'esplosione di fuoco travolge l'area, infliggendo 8d6 danni da fuoco.
traits:
  - name: Incantatore
    desc: Il mago è un incantatore di 6° livello. Ha 4 slot incantesimo di 1° livello, 3 di 2° livello e 3 di 3° livello.
  - name: Scolpire Incantesimi (6° livello, Evocazione)
    desc: Quando lanci un incantesimo di evocazione che infligge danni, puoi creare una sacca di sicurezza vuota attorno a te o a un alleato. Fino a 1 + il livello dell'incantesimo, le creature scelte passano il loro tiro salvezza e non subiscono danni.
  - name: Sfera del Comando Elementale
    desc: Questo oggetto magico permette a Richard di lanciare l'incantesimo “Evoca Elementale” due volte per riposo lungo, senza consumare uno slot incantesimo.
actions:
  - name: Bastone
    desc: "Attacco con Arma da Mischia: +2 al tiro per colpire, portata 1,5 m, un bersaglio. Colpisce: 2 (1d6 - 1) danni contundenti. Versatile (1d8) se impugnato a due mani."
legendary_actions:
  - name: Risveglio della volontà (1 azione leggendaria)
    desc: "Quando Richard raggiunge 0 punti ferita, può usare un'azione leggendaria per attivare il Risveglio Elementale (Fase 2). Quando questo accade, Richard recupera 20 punti ferita temporanei e il suo corpo è avvolto da un'energia elementale. Per 1 minuto, i suoi incantesimi d'evocazione non richiedono concentrazione. Questa azione può essere usata solo una volta."
reactions:
  - name:
    desc: ""
  - name:
    desc: ""
source: Homebrew
modifier: 0

```