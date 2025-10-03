---
Type: Player
Level: 1
AC: 13
Prof: 2
HP: 14
HitDice: d10
Speed: 9
STR: 16
DEX: 13
CONST: 14
INT: 8
WIS: 8
CHA: 12
Race: Draconide Rosso
Stato: In Vita
Alignment: 
Gender: Maschio
Age: 
Taglia: Media
Location: 
Class: Barbaro
Subclass: 
AssociatedGroup: 
Likes: 
Dislikes: 
PersonalityTrait: 
SocialTrait: 
MentalTrait: 
Resistances: 
Proficiencies: 
Languages:
  - Draconide, Gigantesco, Comune
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
  - Spadone di Piombo
Items: 
Spells:
---

## Backstory

Nato e cresciuto in un mini villaggio isolato di dragonidi. 
Quando era ancora un bambino, il villaggio è attaccato da un gruppo di giganti, che lo radono al suolo. Quasi tutti gli abitanti vengono massacrati, ma Carcasso riesce a mettersi in salvo, e viene salvato da un gigante di nome Grog, che lo porta nella sua città e lo istruisce secondo le tradizioni dei giganti. Carcasso, tuttavia, dai giganti acquisisce solo l'ossessione al diventare sempre più forte, e in lui si annida un senso di invidia , causata dal suo senso di inferiorità, verso la razza assassina della sua famiglia ma che allo stesso lo ha salvato.
Molto precipitoso nelle conclusioni, è ossessionato dal concetto che la forza di una persona dipende unicamente da quanto grande è la sua arma, forse sintomo del suo senso di impotenza durante l'assalto al suo villaggio.
Compiuti 15 anni,  decide di rubare uno spadone destinato al successore della guida dei giganti e fugge. L'arma però è troppo grande, e fatica ad usarla correttamente, ma non riesce a disfarsene, vittima di una relazione di amore e odio verso i giganti. Passa quindi un paio d'anni in cerca di altre armi che possano rivaleggiare con lo spadone dei giganti ( e che lui possa usare più facilmente), e ne analizza il contenuto, stilando una guida molto dettagliata di ogni arma che gli capita sotto il naso. Il suo obiettivo è di trovare un'arma unica, e di diventare un guerriero unico nel suo genere, l'unico a poter brandire armi leggendarie; solo in questo modo egli potrà definirsi veramente "forte", e avrà la sicurezza di non dover più scappare da uno scontro.


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