---
Type: NPC
Level: 4
AC: 14
Prof: 2
HP: 26
HitDice: d8
Speed: 10 metri
STR: 8
DEX: 14
CONST: 13
INT: 10
WIS: 17
CHA: 12
Race: Wood Elf
Stato: In Vita
Alignment: Neutral Good
Gender: Femmina
Age: "80"
Location: Foresta di [[Pontevivo]]
Class: Druido
Subclass: Circle of the Land (Forest)
AssociatedGroup: Circle of the Whispering Woods
Likes: Ancient trees, the sound of flowing water, small forest creatures, natural balance, secluded clearings.
Dislikes: Poachers, deforestation, unnatural magic, urban sprawl, industrial sounds.
Pronouns: She/Her
PersonalityTrait:
  - Quietly observant, preferring to listen to nature than engage in idle chatter.
  - Fiercely protective of her forest home and its inhabitants.
SocialTrait:
  - Cautious around strangers, but will offer aid to those in obvious need.
  - More comfortable interacting with animals than with people, often speaking in calming tones to both.
MentalTrait:
  - Possesses a deep, intuitive understanding of natural cycles and magic, seeing connections others miss.
  - Can be stubborn when her principles regarding nature are challenged, refusing to compromise.
Resistances:
  - Nessuna (gli elfi dei boschi non hanno resistenze innate specifiche)
Proficiencies:
  - Light Armor, Medium Armor, Shields, Clubs, Daggers, Javelins, Maces, Quarterstaffs, Scimitars, Sickles, Slings, Spears, Insight, Nature
Languages:
  - Common, Elvish, Sylvan
DmgTkn: 0
TempHP: 0
Copper: 0
Silver: 0
Electrum: 0
Gold: 0
Platinum: 0
---

## Backstory
Druido che vive nella foresta di [[Pontevivo]] e si mantiene neutrale verso tutti. Ha un contratto con i villici per dare loro alberi da tagliare. Non ha un vincolo di protezione verso [[Pontevivo]], ma ha preso in simpatia alcune persone che vede come amici e/o discepoli da allevare.




>[!column|flex 2]
>> [!infobox]
>> # `=this.file.name`
>> ![[Euris.png]]
>> ###### Stats
>>  |
>> ---|---|
>> **Level** |`=this.level` |
>>  **Speed** |`=this.Speed` |
>> **Proficiency** | +`=this.Prof` |
>> **Initiative** | +`=floor((this.DEX - 10)/2)` |
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
| Copper         | Silver         | Gold         | Platinum         |
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
| <font color="#ffff00">**DEX**</font>   | `=this.DEX`  | `=floor((this.DEX - 10)/2)`   | <input type="checkbox" unchecked> | +`=floor((this.DEX - 10)/2)`               |
| <font color="#00b050">**CON**</font>   | `=this.CONST` | `=floor((this.CONST - 10)/2)` | <input type="checkbox" unchecked>   | `=floor((this.CONST - 10)/2)` |
| <font color="#7030a0">**INT**</font>   | `=this.INT`          | `=floor((this.INT - 10)/2)`   | <input type="checkbox" unchecked>   | +`=floor(((this.INT - 10)/2))`   |
| <font color="#245bdb">**WIS**</font>   | `=this.WIS`          | `=floor((this.WIS - 10)/2)`   | <input type="checkbox" unchecked> | +`=floor((this.WIS - 10)/2)`               |
| <font color="#de7802">**CHA**</font>   | `=this.CHA`          | `=floor((this.CHA - 10)/2)`   | <input type="checkbox" unchecked> | +`=floor((this.CHA - 10)/2)`               |
>> ### Skill Checks
| Ability               |                                   | Mod |
| --------------------- | --------------------------------- | --- |
| Acrobatics (DEX)      | <input type="checkbox" unchecked> | +`=floor((this.DEX - 10)/2)`   |
| Animal Handling (WIS) | <input type="checkbox" unchecked> | +`=floor((this.WIS - 10)/2)`  |
| Arcana (INT)          | <input type="checkbox" unchecked> | +`=floor((this.INT - 10)/2)`  |
| Athletics (STR)       | <input type="checkbox" unchecked> | +`=floor((this.STR - 10)/2)`   |
| Deception (CHA)       | <input type="checkbox" unchecked> | +`=floor((this.CHA - 10)/2)`  |
| History (INT)         | <input type="checkbox" unchecked> | +`=floor((this.INT - 10)/2)`  |
| Insight (WIS)         | <input type="checkbox" unchecked>   | +`=floor((this.WIS - 10)/2)`  |
| Intimidation (CHA)    | <input type="checkbox" unchecked> | +`=floor((this.CHA - 10)/2)`  |
| Investigation (INT)   | <input type="checkbox" unchecked>   | +`=floor((this.INT - 10)/2)`  |
| Medicine (WIS)        | <input type="checkbox" unchecked> | +`=floor((this.WIS - 10)/2)`  |
| Nature (INT)          | <input type="checkbox" unchecked> | +`=floor((this.INT - 10)/2)`  |
| Perception (WIS)      | <input type="checkbox" unchecked>   | +`=floor((this.WIS - 10)/2)`  |
| Performance (CHA)     | <input type="checkbox" unchecked> | +`=floor((this.CHA - 10)/2)`  |
| Persuasion (CHA)      | <input type="checkbox" unchecked> | +`=floor((this.CHA - 10)/2)`  |
| Religion (INT)        | <input type="checkbox" unchecked> | +`=floor((this.INT - 10)/2)`  |
| Sleight of Hand (DEX) | <input type="checkbox" unchecked> | +`=floor((this.DEX - 10)/2)`   |
| Stealth (DEX)         | <input type="checkbox" unchecked> | +`=floor((this.DEX - 10)/2)`   |
| Survival (WIS)        | <input type="checkbox" unchecked> | +`=floor((this.WIS - 10)/2)`  |
