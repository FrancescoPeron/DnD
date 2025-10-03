---
Type: Player
Level: 1
AC: 13
Prof: 2
HP: 8
HitDice: 0
Speed: 9
STR: 9
DEX: 16
CONST: 14
INT: 17
WIS: 9
CHA: 10
Race: Elfo Alto
Taglia: Media
Stato: In Vita
Alignment: 
Gender: Femmina
Age: 
Location: 
Class: Mago
Subclass: Evocatore(?)
AssociatedGroup: 
Likes: 
Dislikes: 
PersonalityTrait: 
SocialTrait: 
MentalTrait: 
Resistances: 
Proficiencies: 
Languages:
  - Comune, Elfico
DmgTkn: 0
TempHP: 0
Copper: 0
Silver: 0
Electrum: 0
Gold: 0
Platinum: 0
Armor:
  - Vestiario
Weapon:
  - Pugnale, Bastone ferrato
Items: 
Spells:
---

## Backstory

Alfea è una giovane maga con l'odio per i carretti e l'amore per le esplosioni.
Ha studiato in accademia di magia passando quasi interamente tutto il suo tempo in biblioteca e quindi avendo poco a che fare con le altre "persone".
Quando non era in accademia, cercava di tornare a casa e per farlo doveva arrendersi e prendere un carretto che però, inevitabilmente, aveva dei problemi. Ritardi, rotture o cancellazioni.
In accademia gli incantesimi di esplosione non sono ben visti perché pericolosi e quindi ne vengono insegnati solo di facili e raramente permettono di metterli alla prova.
Alfea quindi è curiosa di scoprire se, al di fuori della accademia, qualcuno usi incantesimi di esplosione più complessi così da poter finalmente sfogare un animo represso contro i carretti.

Perché ha deciso di partire all'avventura? musica triste
Semplicemente perché tra biblioteca e carretti non ha quasi mai interagito con altri esseri e quindi questa è la sua occasione per scoprire "persone nuove".
Avendo paura e all'inizio poche risorse, spesso ricorre alla fuga ma i compagni di avventura sono comunque le prime persone che conosce quasi quindi diventa protettiva al costo di tutti quelli che cercano di ostacolarli. 
Come comportamenti è quindi un misto tra attacco e fuga

>[!column|flex 2]
>> [!infobox]
>> # `=this.file.name`
>> ![[Character Image Placeholder]]
>> ###### Stats
>>  |
>> ---|---|
>> **Level** |`=this.level` |
>>  **Speed** |`=this.Speed` |
>> **Proficiency** | +`=this.Prof` |
>> **Initiative** | `=floor((this.DEX - 10)/2)` |
>> **AC** | `=this.AC`
>> **HP** | `=this.HP - this.DmgTkn + this.TempHP` |
>> **Hit Dice** | `=this.Level + this.HitDice`  |
>> **Passive Perception** | `=10 + floor((this.DEX - 10)/2)`|
>>  
>> ###### Bio
>>   |
>> ---|---|
>> **Race** | `=this.race` |
>> **Sex** | `=this.gender` |
>> **Age** | `=this.age` |
>> **Sexuality** | `=this.sexuality` |
>> **Alignment** | `=this.alignment` |
>> ###### Info
>>   |
>> ---|---|
>> **Class(s)** | `=this.Class` |
>> **Sub-Class(s)** | `=this.Subclass`
>> **Group(s)** | `=this.AssociatedGroup` |
>> **Religion(s)** | `=this.AssociatedReligion` |
>> **Current Location** | `=this.Location` |
>>  ### Currency
| Copper   | Silver    | Gold      | Plat        |
| -------------- | -------------- | ------------ | ---------------- |
| `=this.Copper` | `=this.Silver` | `=this.Gold` | `=this.Platinum` |
>
>> [!infobox] Death Saves
>> ### Death Saves
| Success | <input type="checkbox" unchecked>  | <input type="checkbox" unchecked> | <input type="checkbox" unchecked> | 
| ------- | --- | --------------------------------- | --------------------------------- |
>>
| Fails | <input type="checkbox" unchecked>  | <input type="checkbox" unchecked> | <input type="checkbox" unchecked> | 
| ----- | --- | --------------------------------- | --------------------------------- |
>>
>> ### Skills
| Skill | Score       | Mod                     | Prof                              | ST                                  |
| ----- | ----------- | ----------------------- | --------------------------------- | ----------------------------------- |
| <font color="#ff0000">**STR**</font>   | `=this.STR` | `=floor((this.STR - 10)/2)`  | <input type="checkbox" unchecked> | `=floor((this.STR - 10)/2)`               |
| <font color="#ffff00">**DEX**</font>   | `=this.DEX`  | `=floor((this.DEX - 10)/2)`   | <input type="checkbox" unchecked> | `=floor((this.DEX - 10)/2)`               |
| <font color="#00b050">**CON**</font>   | `=this.CONST` | `=floor((this.CONST - 10)/2)` | <input type="checkbox" unchecked>   | `=floor((this.CONST - 10)/2)` |
| <font color="#7030a0">**INT**</font>   | `=this.INT`          | `=floor((this.INT - 10)/2)`   | <input type="checkbox" unchecked>   | `=floor(((this.INT - 10)/2))`   |
| <font color="#245bdb">**WIS**</font>   | `=this.WIS`          | `=floor((this.WIS - 10)/2)`   | <input type="checkbox" unchecked> | `=floor((this.WIS - 10)/2)`               |
| <font color="#de7802">**CHA**</font>   | `=this.CHA`          | `=floor((this.CHA - 10)/2)`   | <input type="checkbox" unchecked> | `=floor((this.CHA - 10)/2)`               |
>> ### Skill Checks
| Ability               |                                   | Mod |
| --------------------- | --------------------------------- | --- |
| Acrobatics (DEX)      | <input type="checkbox" unchecked> | `=floor((this.DEX - 10)/2)`   |
| Animal Handling (WIS) | <input type="checkbox" unchecked> | `=floor((this.WIS - 10)/2)`  |
| Arcana (INT)          | <input type="checkbox" unchecked> | `=floor((this.INT - 10)/2)`  |
| Athletics (STR)       | <input type="checkbox" unchecked> | `=floor((this.STR - 10)/2)`   |
| Deception (CHA)       | <input type="checkbox" unchecked> | `=floor((this.CHA - 10)/2)`  |
| History (INT)         | <input type="checkbox" unchecked> | `=floor((this.INT - 10)/2)`  |
| Insight (WIS)         | <input type="checkbox" unchecked>   | `=floor((this.WIS - 10)/2)`  |
| Intimidation (CHA)    | <input type="checkbox" unchecked> | `=floor((this.CHA - 10)/2)`  |
| Investigation (INT)   | <input type="checkbox" unchecked>   | `=floor((this.INT - 10)/2)`  |
| Medicine (WIS)        | <input type="checkbox" unchecked> | `=floor((this.WIS - 10)/2)`  |
| Nature (INT)          | <input type="checkbox" unchecked> | `=floor((this.INT - 10)/2)`  |
| Perception (WIS)      | <input type="checkbox" unchecked>   | `=floor((this.WIS - 10)/2)`  |
| Performance (CHA)     | <input type="checkbox" unchecked> | `=floor((this.CHA - 10)/2)`  |
| Persuasion (CHA)      | <input type="checkbox" unchecked> | `=floor((this.CHA - 10)/2)`  |
| Religion (INT)        | <input type="checkbox" unchecked> | `=floor((this.INT - 10)/2)`  |
| Sleight of Hand (DEX) | <input type="checkbox" unchecked> | `=floor((this.DEX - 10)/2)`   |
| Stealth (DEX)         | <input type="checkbox" unchecked> | `=floor((this.DEX - 10)/2)`   |
| Survival (WIS)        | <input type="checkbox" unchecked> | `=floor((this.WIS - 10)/2)`  |


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

dv.header(4, "Incantesimi:");
let Spellitems = dv.current().Spells; 
if (Spellitems) { 
    if (!Array.isArray(Spellitems)) {
        Spellitems = [Spellitems]; 
    }

    
    Spellitems.forEach(item => {
        dv.el("li", item); 
    });
} else {
    dv.paragraph("Nessun incantesimo specificato.");
}