
## DCS World - NOTAM

Notice to Airmen: A written notification issued to pilots before flight concerning the establishment, conditions or change in any aeronautical facility, service, procedure or hazard, the timely knowledge of which may be essential to personnel and systems concerned with flight operations.

**Why?**
Because in my opinion it is preferable to know your options during planning time, i.e. what works and to what extent, instead of having to find out the hard way: over the target area after 1.5 h mission time (or trial & error).
  
**Is it realistic?**
Not only is the study of NOTAM part of any real life briefing, but in DCS World it may have the added value of preventing one from running into odd quirks during a mission. In a way, NOTAM might even make DCS quirks look like a realistic part of the simulation.
  
**How is this different from a bug list?**
A bug list features all things that remain to be corrected, f.ex. graphical issues, omissions etc. This is not the idea of NOTAM. Also the presentation here is more systematic than ED's bugs sections.
  
**What should go into NOTAM?**
Focus should be set on operationally relevant issues. Real world NOTAM can serve as a good example (sometimes...)
  
**How could this be done?**
Obviously this can only be achieved as a group effort. Github is a good starting point, because of its accessibility, but this project could move to another platform in the future.

### NOTAM Formatting Rules ###
#### Entries
**1st line: ID**  
date formatted like this \<yymmdd> followed by \'-' + \<code> + number  
codes:

| | |
|---|---|
|CA|Caucasus|
|MA|Marianas|
|NE|Nevada|
|PG|Persian Gulf|
|SA|South Atlantic|
|SI|Sinai|
|SY|Syria|

number: start every day's first entry with '1', and increment every new entry of that day and theater  

**2nd line: DESCRIPTION**  
prefer concise style using appropriate abbreviations, when possible. Typically start with concerned item, followed by issue. Terminate with '.'  

#### Sorting
o theaters alphabetically  
o airports alphabetically  
o entries by date of entry  
***
## DCS World - Hold Item List
Hold Item List: A list of specific maintenance work orders that are deferred, because a required part, piece of equipment or system is either missing or inoperable although a limitation might be associated with the HIL record. In simpler terms: DCS_HIL lets you check current status/airworthiness of your DCS aircraft, before you hop in or start planning your next mission. It's the way it's done in real life.

**Why?**
Because in my opinion it is preferable to know your options during planning time, i.e. what works and to what extent, instead of having to find out the hard way: over the target area after 1.5 h mission time (or trial & error).

**Is it realistic?**
Real life aircraft often have small defects that dont require immediate grounding. Flight & maintenance crews use the manufacturer's documentation to assess, if and under which conditions an aircraft is airworthy, before flight. So in a way software bugs or broken/missing features could even be considered as realistic part of the simulation. 

**How is this different from a bug list?**
A bug list features all things that remain to be corrected, f.ex. graphical issues/missing sounds, and things that may not be in line with their real counterpart, whether or not those things are impeding basic functionality. Also the HIL presents relevant defects in a more systematic form than the bugs sections in ED's forums.

**What should go into the HIL?**
Only items or essential features that are originally part of the module modeled, but are broken or completely missing (that would prevent a specific task to be performed as expected). Also a workaround, if available. The source should ideally provide a link to a discussion thread that allows easy tracking of the defect's current state.
**Reference: official game manual or Chuck's guides** as a general rule. -I think there is no point in browsing through real life docs, and listing everything that's missing in the game.

**How could this be done?**
Obviously this can only be achieved as a group effort. Github is a good starting point, because of its accessibility, but this project could move to another platform in the future.

### HIL Formatting Rules ###
The **MISSION PROFILE / PERFORMANCE** table is supposed to give the user a quick overview of his aircraft's current capabilities (actually inabilities). Only applicable and restricted capabilities should be listed here, and the header line be labeled accrodingly either/or
| **unrestricted** |**`RESTRICTED`**|
| --- | --- |

The **REFER TO** section should point to the concerned CATEGORY, further details be given therein.

**CATEGORIES** (Flight Control System, Weapon System, etc.) are always listed, except if not applicable to the aircraft, and labeled according to the following rule: if at least one item is either RESTRICTED or INOP, the whole CATEGORY is labelled RESTRICTED; otherwise UNRESTRICTED
| **unrestricted** |**`RESTRICTED`**|
| --- | --- |

**ITEMS** (Speedbrake, AIM-120C, etc.) are only listed, if restricted (workaround may be available) or inoperative (completely unusable or missing feature), and labeled as follows
|**`RESTRICTED`**|**`INOP`**|
|--- | --- |

**[F]** indicates the feature is completely missing (although it could reasonably be expected) or intended as is (although evidence indicates otherwise)

**[B]** indicates the feature is technically implemented, but bugged/broken

**Dates:**
- use full year within header, i.e. 2022
- use 2-digit year in subcategories, i.e. 23

**Sorting:**
- categories by priority, see template below (do not change)
- items alphabetically; except for weapon system: air-air weapons first, alphabetically, air-ground weapons next, also alphabetically

### Template ###
Use this as example or template. Listed ITEMS are exemplary only, and not extensive.
***
## HOLD ITEM LIST

| A/C Type | A/C Serial No | Release Date | Company |
| --- | --- | --- | --- |
| xxx | xxx | yyyy-mm-dd | xxxx |

||||||
| --- | --- | --- |--- | --- |
| Document Created by: xxx | Release Date: yyyy-mm-dd || Last Edit: xxx | Date: yyyy-mm-dd |
***
| **Mission Profile / Performance** | **unrestricted** ||||
| --- | --- | --- | --- | --- |
| *Item* | *Restriction* | *Refer to* | *Entry by* | *Date* |
| Takeoff | --- | --- | --- | --- |
| Landing | --- | --- | --- | --- |
| VFR | --- | --- | --- | --- |
| IFR | --- | --- | --- | --- |
| TOT | --- | --- | --- | --- |
| AA | --- | --- | --- | --- |
| AG | --- | --- | --- | --- |
| Recon | --- | --- | --- | --- |
| Rescue | --- | --- | --- | --- |
| Transport | --- | --- | --- | --- |
| Range | --- | --- | --- | --- |
| Air Air Refueling | --- | --- | --- | --- |
| Cold Weather Operation | --- | --- | --- | --- |
| Night Operation | --- | --- | --- | --- |
| Carrier Operation | --- | --- | --- | --- |
***
| **Flight Control Systems** | **`RESTRICTED`** ||||
| --- | --- | --- | --- | --- |
| *Item* | *Restriction* | *Description / Workaround / Source* | *Entry by* | *Date* |
| Fly by Wire System | --- | --- | --- | --- |
| Flaps | --- | --- | --- | --- |
| Trim | --- | --- | --- | --- |
| Example | **`INOP`** | very very long description and even longer workaround 1234567890 1234567890 1234567890 1234567890 1234567890 1234567890 1234567890 1234567890 1234567890 1234567890 1234567890 1234567890 1234567890 1234567890 1234567890 1234567890 1234567890 1234567890 1234567890 1234567890 1234567890 1234567890 1234567890 1234567890 1234567890 1234567890 1234567890 1234567890 1234567890 1234567890 1234567890 1234567890 1234567890 1234567890 1234567890 1234567890 1234567890 1234567890 1234567890 1234567890 | HILOK | 2021-11-24 |

| **Powerplant** | **unrestricted** ||||
| --- | --- | --- | --- | --- |
| *Item* | *Restriction* | *Description / Workaround / Source* | *Entry by* | *Date* |
| APU | --- | --- | --- | --- |
| Engine#4 | --- | --- | --- | --- |

| **Aircraft Systems** | **unrestricted** ||||
| --- | --- | --- | --- | --- |
| *Item* | *Restriction* | *Description / Workaround / Source* | *Entry by* | *Date* |
| Hydraulics | --- | --- | --- | --- |
| Electrics | --- | --- | --- | --- |
| Pneumatics | --- | --- | --- | --- |
| Fuel | --- | --- | --- | --- |
| Landing Gear | --- | --- | --- | --- |

| **Avionics / Instrumentation** | **unrestricted** ||||
| --- | --- | --- | --- | --- |
| *Item* | *Restriction* | *Description / Workaround / Source* | *Entry by* | *Date* |
| ADF | --- | --- | --- | --- |
| DME | --- | --- | --- | --- |
| GPS | --- | --- | --- | --- |
| ILS | --- | --- | --- | --- |
| INS | --- | --- | --- | --- |
| TACAN | --- | --- | --- | --- |
| Terrain Following | --- | --- | --- | --- |
| VOR | --- | --- | --- | --- |

| **Communication** | **unrestricted** ||||
| --- | --- | --- | --- | --- |
| *Item* | *Restriction* | *Description / Workaround / Source* | *Entry by* | *Date* |
| Datalink | --- | --- | --- | --- |
| FM | --- | --- | --- | --- |
| HF | --- | --- | --- | --- |
| IFF | --- | --- | --- | --- |
| UHF | --- | --- | --- | --- |
| VHF | --- | --- | --- | --- |

| **Defensive Systems** | **unrestricted** ||||
| --- | --- | --- | --- | --- |
| *Item* | *Restriction* | *Description / Workaround / Source* | *Entry by* | *Date* |
| --- | --- | --- | --- | --- |

| **Targeting / Aiming Systems** | **unrestricted** ||||
| --- | --- | --- | --- | --- |
| *Item* | *Restriction* | *Description / Workaround / Source* | *Entry by* | *Date* |
| --- | --- | --- | --- | --- |

| **Weapon Systems** | **unrestricted** ||||
| --- | --- | --- | --- | --- |
| *Item* | *Restriction* | *Description / Workaround / Source* | *Entry by* | *Date* |
| Gun | --- | --- | --- | --- |
| AIM-7F | --- | --- | --- | --- |
| AIM-120C | --- | --- | --- | --- |
| CAP-9M | --- | --- | --- | --- |
| AGM-62 | --- | --- | --- | --- |
| AGM-154C | --- | --- | --- | --- |
| BDU-33 | --- | --- | --- | --- |
| CBU-99 | --- | --- | --- | --- |
| GBU-12 | --- | --- | --- | --- |
| GBU-31 | --- | --- | --- | --- |
| Mk. 5 | --- | --- | --- | --- |
| Mk. 151 | --- | --- | --- | --- |

| **Equipment** | **unrestricted** ||||
| --- | --- | --- | --- | --- |
| *Item* | *Restriction* | *Description / Workaround / Source* | *Entry by* | *Date* |
| De-Icing | --- | --- | --- | --- |
| Fire Detection | --- | --- | --- | --- |
| Position Lights | --- | --- | --- | --- |
***
- EOF
