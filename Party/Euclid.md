---
Type: Player
Art: Halfling.png
Level: 1
AC: 0
Prof: 0
HP: 0
HitDice: 0
Speed: 0
STR: 0
DEX: 0
CONST: 0
INT: 0
WIS: 0
CHA: 0
Race: Halfling
Stato: In Vita
Alignment: 
Gender: Maschio
Age: 
Location: 
Class: Bardo
Subclass: Collegio dell'Eloquenza
AssociatedGroup: 
Likes: 
Dislikes: 
PersonalityTrait: 
SocialTrait: 
MentalTrait: 
Resistances: 
Proficiencies: 
Languages: 
DmgTkn: 0
TempHP: 0
Copper: 0
Silver: 0
Electrum: 0
Gold: 0
Platinum: 0
Armor: 
Weapon: 
Items: 
Spells:
---

## Backstory
Orfano dei genitori (sa solo che sono morti in maniera violenta), è stato allevato in un circo dove ha sviluppato le capacità acrobatiche, i genitori adottivi gli hanno insegnato a farsi voler bene. Fin dalla tenera età gli piace raccontare storie anche inventate, non sa né leggere né scrivere, ma vuole diventare capace di raccontare avventure delle quali è il protagonista. Vuole sapere il più possibile, la sua curiosità l’ha cacciato molte volte nei guai ma i piedi veloci e la stazza lo hanno reso in grado di fuggire sempre. Da qualche anno cresce un mastino Rubeus.

Non importa come. ma userà ogni sua conoscenza per piegare la trama della realtà al suo volere, scoprire cos’è successo ai suoi genitori e fare in modo che non succeda a nessun altro. E’ importante per lui che non muoia nessuno a cui tiene.




>[!column|flex 2]
>> [!infobox]
>> # `=this.file.name`
>> ![[Halfling.png]]
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