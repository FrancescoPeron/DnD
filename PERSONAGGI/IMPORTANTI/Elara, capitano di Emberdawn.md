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
  - Armatura Completa (CA 18) Ben mantenuta e lucida, riflette la sua devozione.
Weapon:
  - Spada Lunga 1d8/1d10 (taglienti), Versatile, Fedele compagna in innumerevoli battaglie.
  - Martello da Guerra, 1d8/1d10 (contundenti) Versatile, Arma secondaria per forza bruta o difese robuste.
Items:
  - Simbolo Sacro, Medaglione d'argento raffigurante un'aquila, emblema del suo ordine.
  - Kit da Viaggiatore, Contiene provviste per un giorno, coperta, scatola per l'esca, tazza, posate, borsa, fune da 15m.
  - Borraccia, Piena d'acqua fresca.
  - Razione da Viaggio, per 3 giorni
  - Mappa di Emberdawn e dintorni, Dettagliata delle aree che protegge e percorsi pattugliati.
  - Diario di Cuoio e Carbone, Piccolo diario per osservazioni, pensieri e resoconti delle missioni.
  - Fiala di Acqua Santa, Utile contro le creature delle tenebre.
---


## Backstory
Elara non è sempre stata il capitano risoluto e devoto che è oggi. La sua lunga vita, un dono o forse un fardello della sua eredità celestiale parziale, l'ha vista testimone di innumerevoli albe e tramonti sulla città di [[Emberdawn]]. Nata in una stirpe di antichi protettori del regno, Elara è stata cresciuta con i racconti di giustizia e sacrificio, principi che presto sarebbero diventati la sua stessa guida.

Da giovane paladina, Elara si è distinta per la sua incrollabile fede e il suo coraggio in battaglia. Il suo giuramento di devozione non era solo una formula recitata, ma una promessa scolpita nella sua anima, plasmando ogni sua azione. Ha servito per decenni come guardiano di [[Emberdawn]], difendendo i suoi confini da minacce sia terrene che ultraterrene. È stata il faro di speranza durante assedi, la lama che ha spezzato l'oscurità in antiche rovine e la voce che ha portato conforto nei momenti di disperazione.


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
name: Elara
image: [[female_orc_paladin.webp]]
layout: Basic 5e Layout Better
size: Media
type: Umanoide
subtype: Orco
alignment: Legale Buono
ac: 19 
hp: 36
hit_dice: 4d10
speed: 9m
stats: [16, 10, 14, 8, 12, 15]
saves:
- Destrezza: 2
- Costituzione: 4
- Saggezza: 3
- Carisma: 4
skillsaves:
- Intuizione: 3
- Persuasione: 4
- Atletica: 5
damage_vulnerabilities: ""
damage_resistances: ""
damage_immunities: ""
condition_immunities: ""
senses: Percezione Passiva 12
languages: Comune, Celestiale
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
    desc: "Elara ha giurato di sostenere i principi di Onestà, Coraggio, Compassione, Onore e Dovere. Queste parole sono la sua guida in ogni azione."
  - name: Senso Divino
    desc: "Come azione, Elara può percepire la presenza di celestiali, immondi o non morti entro 18m per 1 minuto. Può usare questa capacità un numero di volte pari a 1 + il suo modificatore di Carisma (minimo 1), e recupera tutti gli usi dopo un riposo lungo."
  - name: Imposizione delle Mani
    desc: "Elara ha un ammontare di punti di cura pari a 5 x il suo livello da Paladino (20 punti). Come azione, può toccare una creatura e spendere punti per curarla, fino al massimo dei punti rimanenti. In alternativa, può spendere 5 punti per curare una malattia o una condizione di Veleno."
  - name: Stile di Combattimento (Difesa)
    desc: "Mentre indossa un'armatura, Elara ottiene un bonus di +1 alla CA."
actions:
  - name: Spada Lunga a una mano
    desc: "Attacco con arma da mischia: +5 al tiro per colpire, portata 1.5m, un bersaglio. Colpito: 1d8 + 3 danni taglienti."
  - name: Spada Lunga a due mani
    desc: "Attacco con arma da mischia: +5 al tiro per colpire, portata 1.5m, un bersaglio. Colpito: 1d10 + 3 danni taglienti."
  - name: Colpo Divino
    desc: "Quando Elara colpisce una creatura con un attacco con arma da mischia, può spendere uno slot incantesimo per infliggere 2d8 danni radiosi aggiuntivi al bersaglio, più 1d8 per ogni livello di slot incantesimo superiore al 1°. Se il bersaglio è un non morto o un immondo, i danni aumentano di 1d8."
legendary_actions: []
reactions: []

```
