
## DCS World - Hold Item List

Hold Item List: A list of specific maintenance work orders that are deferred, because a required part, piece of equipment or system is either missing or inoperable although a limitation might be associated with the HIL record. In simpler terms: DCS_HIL lets you check current status/airworthiness of your DCS aircraft, before you hop in or start planning your next mission. It's the way it's done in real life.

**Why?**
Because in my opinion it is preferable to know your options during planning time, i.e. what works and to what extent, instead of having to find out the hard way: over the target area after 1.5 h mission time (or trial & error).

**Is it realistic?**
Real life aircraft often have small defects that dont require immediate grounding. Flight & maintenance crews use the manufacturer's documentation to assess, if and under which conditions an aircraft is airworthy, before flight. So in a way software bugs or broken/missing features could even be considered as realistic part of the simulation. 

**How is this different from a bug list?**
A bug list features all things that remain to be corrected, f.ex. graphical issues/missing sounds, and things that may not be in line with their real counterpart, whether or not those things are impeding basic functionality. Also the HIL presents relevant defects in a more systematic form than the bugs sections in ED's forums.

**What should go into the HIL?**
Only items or essential features that are originally part of the module modeled, but are broken or completely missing (that would prevent a specific task to be performed as expected). Also a workaround, if available. The source should ideally provide a link to a discussion thread that allows easy tracking of the defect's current state
**Reference: official game manual or Chuck's guides** as a general rule. -i think there is no point in browsing through real life docs, and listing everything that's missing in the game.

**How could this be done?**
Obviously this can only be achieved as a group effort. Github is a good starting point, because of its accessibility, but this project could move to another platform in the future.

### Formatting Rules ###
The **MISSION PROFILE / PERFORMANCE** table is supposed to give the user a quick overview of his aircraft's current capabilities. Only applicable capabilities should be listed here, and, depending on ITEMS below, be labeled either/or
| **unrestricted** |**`RESTRICTED`**|
| --- | --- |

The **REFER TO** section should point to the concerned CATEGORY, further details be given therein.

**CATEGORIES** (Flight Control System, Weapon System, etc.) are always listed, except if not applicable to the aircraft (e.g. targeting system in the Huey), and labeled according to the following rule: if at least one item is either RESTRICTED or INOP, the whole CATEGORY is labelled RESTRICTED; otherwise UNRESTRICTED
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

| **Targeting Systems** | **unrestricted** ||||
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
