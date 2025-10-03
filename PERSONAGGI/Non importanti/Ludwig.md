---
Type: NPC
Stato: In Vita
Gender: Maschio
Age: 33 anni
Location: Pontevivo
AssociatedGroup: Nessuno
Copper: 10
Silver: 20
Electrum: 0
Gold: 0
Platinum: 0
Armor:
  - Armatura Completa (AC 18)
Weapon:
  - Spada Lunga, 1d8 taglienti (Versatile 1d10)
  - Martello da Guerra, 1d8 contundenti (Versatile 1d10)
Items:
  - Simbolo Sacro (Medaglione)
  - Kit da Viaggiatore
  - Borraccia
  - Razione da Viaggio (3 giorni)
  - Mappa di Pontevivo e dintorni
  - Diario di Cuoio e Carbone
  - Fiala di Acqua Santa
---

## Backstory
Ludwig ha sempre vissuto onestamente ed è aperto di mente. Ha cominciato la sua carriera militare come soldato, ma dopo essersi sposato si è trasferito come guardia di [[Pontevivo]], e successivamente ne è diventato il capo delle guardie. Cerca di evitare sempre un conflitto che coinvolga i civili, e tiene a cuore la vita dei suoi sottoposti. Ha un figlio di tre anni.

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
name: Ludwig
layout: Basic 5e Layout Better
size: Media
type: Umanoide
subtype: Umano
alignment: Legale Buono
ac: 18
hp: 30
hit_dice: 3d10
speed: 9m
stats: [16, 10, 14, 12, 10, 14]
saves:
- Destrezza: 0
- Costituzione: 2
- Saggezza: 2
- Carisma: 4
skillsaves:
- Intuizione: 2
- Persuasione: 4
- Atletica: 5
damage_vulnerabilities: ""
damage_resistances: ""
damage_immunities: ""
condition_immunities: ""
senses: Percezione Passiva 10
languages: Comune
cr: 2
spellnotes: CHA (+4), CD 12
spells:
  - name: Benedizione
    desc: "Come azione, puoi toccare una creatura a tua scelta. Il bersaglio ottiene un bonus di 1d4 a tutti i tiri per colpire e ai tiri salvezza fino alla fine del tuo prossimo turno."
  - name: Scudo della Fede
    desc: "Come azione bonus, puoi toccare una creatura entro 1,5 metri. La CA del bersaglio aumenta di 2 fino a quando l'incantesimo non termina o finché non perdi la concentrazione (fino a 1 minuto)."
  - name: Cura Ferite
    desc: "Come azione, puoi toccare una creatura. Il bersaglio recupera 1d8 + il tuo modificatore di Carisma (1d8 + 2) punti ferita."
  - name: Individuazione del Magico
    desc: "Come azione, puoi usare i tuoi sensi per percepire la magia. Fino alla fine del tuo prossimo turno, puoi vedere un'aura debole attorno a qualsiasi creatura o oggetto entro 9 metri che possiede magia, e sai a quale scuola di magia appartiene. L'incantesimo richiede concentrazione (fino a 10 minuti)."
  - name: Protezione dal Bene e dal Male
    desc: "Come azione, puoi toccare una creatura. Fino a quando l'incantesimo non termina o finché non perdi la concentrazione (fino a 10 minuti), il bersaglio non può essere affascinato, spaventato o posseduto da celestiali, elementali, folletti, immondi e non morti. Inoltre, questi tipi di creature hanno svantaggio ai tiri per colpire contro il bersaglio."
traits:
  - name: Giuramento di Devozione
    desc: "Ludwig ha giurato di sostenere i principi di Onestà, Coraggio, Compassione, Onore e Dovere. Queste parole sono la sua guida in ogni azione."
  - name: Senso Divino
    desc: "Come azione, Ludwig può percepire la presenza di celestiali, immondi o non morti entro 18m per 1 minuto. Può usare questa capacità un numero di volte pari a 1 + il suo modificatore di Carisma (minimo 1), e recupera tutti gli usi dopo un riposo lungo."
  - name: Imposizione delle Mani
    desc: "Ludwig ha un ammontare di punti di cura pari a 5 x il suo livello da Paladino (15 punti). Come azione, può toccare una creatura e spendere punti per curarla, fino al massimo dei punti rimanenti. In alternativa, può spendere 5 punti per curare una malattia o una condizione di Veleno."
  - name: Stile di Combattimento (Difesa)
    desc: "Mentre indossa un'armatura, Ludwig ottiene un bonus di +1 alla CA."
actions:
  - name: Spada Lunga a una mano
    desc: "Attacco con arma da mischia: +5 al tiro per colpire, portata 1.5m, un bersaglio. Colpito: 1d8 + 3 danni taglienti."
  - name: Spada Lunga a due mani
    desc: "Attacco con arma da mischia: +5 al tiro per colpire, portata 1.5m, un bersaglio. Colpito: 1d10 + 3 danni taglienti."
  - name: Colpo Divino
    desc: "Quando Ludwig colpisce una creatura con un attacco con arma da mischia, può spendere uno slot incantesimo per infliggere 2d8 danni radiosi aggiuntivi al bersaglio, più 1d8 per ogni livello di slot incantesimo superiore al 1°. Se il bersaglio è un non morto o un immondo, i danni aumentano di 1d8."
legendary_actions: ""
reactions: ""

```