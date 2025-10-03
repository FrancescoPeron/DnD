---
Type: Player
Level: 1
AC: 14
Prof: 2
HP: 9
HitDice: 0
Speed: 9
STR: 9
DEX: 14
CONST: 12
INT: 11
WIS: 13
CHA: 17
Race: Tiefling
Stato: In Vita
Alignment: Caotico Neutrale
Gender: Maschio
Age: 27 anni
Location: 
Class: Warlock
Subclass: Giasia
AssociatedGroup: 
Likes: 
Dislikes: 
PersonalityTrait: 
SocialTrait: 
MentalTrait: 
Resistances: 
Proficiencies: 
Languages:
  - Comune, Infernale, Elfico
DmgTkn: 0
TempHP: 0
Copper: 0
Silver: 0
Electrum: 0
Gold: 0
Platinum: 0
Armor:
  - Armatura di cuoio
Weapon:
  - Pugnale
Items: 
Spells:
---

## Backstory
Un giovane avventuriero, nato umano, amante di conoscenza e potere.
Dentro un dungeon infernale si trova faccia a faccia con Belzebu. Asmodeus acde vittima di una trappola di Belzebu per accontentare la sua voglia di potere, e riceve il sangue di Belzebu, con il quale si trasforma in un tiefling.
In preda alla disperazione per cercare di tornare umano, si riversa nella ricerca di conoscenza antica, in quanto quella moderna non lo può aiutare. Durante questa sua ricerca si imbatte in "Oghma Infinium", un tomo primordiale che permette il contatto con la divinità daedrica del sapere [[Haermaus Mora]]. [[Asmodeus]] accetta l'offerta di diventare un aspirante campione della divinità, in cambio di ottenere accesso alla libreria del sapere una volta diventato ufficialmente campione.



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