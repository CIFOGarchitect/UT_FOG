# Utah Interoperable Communications Field Operations Guide
## Version 4.0 — WORKING DRAFT (PRIVATE — CONTROLLED)

**Status:** Working draft, private. Controlled (CUI) — distribution
limited to authorized users. Not for publication and not for
distribution beyond authorized reviewers. Built from known information
on Oct 24, 2026; content is being filled in as it is confirmed.

**Cover (per approved draft):**
- Version 4.0 — January 2027 (planned)
- Authority: Statewide Interoperability Coordinator, under the
  direction of the Statewide Interoperability Executive Committee
- Published by: Statewide Interoperability Coordinator, Utah Division
  of Emergency Management, Department of Public Safety (DPS/DEM)
- Distribution: Controlled (CUI)
- Supersedes: Version 3.0 (November 2022)
- Marking: CUI replaces FOUO throughout (per SWIC direction, Oct 24)

**Section status:** Populated below = Utah Regions, 700 MHz Interop
Talkgroups and Channels (summary + companion file), Radio Template
Programming Requirements (carried forward from v3.0 — VERIFY, to be
updated by the SWIC over winter 2026-27). All other sections
from the v3.0 table of contents remain placeholders pending content
review: Establishing Interoperability, Introduction, State Maps,
Interoperability and Incident Management, Communications Unit (COMU),
Requests for Communications Assets, National Interoperability Channels
(NIFOG), Federal Interoperability Channel Plan, PSAP Information, Nationwide Interop Channel
Capabilities, Statewide Interop Channel Capabilities, Interoperable
Repeaters, Gateways, Transportable Repeaters, Radio Caches, Data
Communications Devices.

---

## Utah Regions (POPULATED — Oct 24, 2026)

Updated from the seven Homeland Security Regions in v3.0 to the
current eight-region structure:

| Code | Region | Counties |
|------|--------|----------|
| BR | Bear River | Box Elder, Cache, Rich |
| WF | Wasatch Front | Weber, Davis, Morgan |
| OQ | Oquirrh | Tooele, Salt Lake |
| MT | Mountain | Summit, Wasatch, Utah, Juab |
| NE | Northeast | Daggett, Duchesne, Uintah |
| CN | Central | Millard, Sanpete, Sevier, Piute, Wayne |
| SW | Southwest | Beaver, Iron, Washington, Garfield, Kane |
| SE | Southeast | Carbon, Emery, Grand, San Juan |

29 counties total. Source: current region map provided by the SWIC,
Oct 24, 2026.

---

## 700 MHz Interop Talkgroups and Channels (POPULATED SUMMARY — Oct 24, 2026)

**Rename note:** In v3.0 this section was titled "800 MHz Interop
Talkgroups and Channels." Per SWIC direction on Oct 24, 2026, it is now
700 MHz. Other 800 MHz references elsewhere in the guide have NOT been
blanket-renamed; each needs individual review.

**Source:** UCA fleet map as provided Oct 24, 2026
(UCA_Fleet_Map.xlsx). Values are preserved verbatim in the companion
file; nothing has been added, removed, or re-valued.

**Companion file:** `utfog-v4-700mhz-talkgroups-organized.csv`
— the full listing, organized by name prefix (new "Group" column) and
sorted by group, then talkgroup name. Columns: Group, Talk Group Name,
Radio Top Display Alias, Motorola Talk Group ID, Encryption, Agency
Restricted Talk Group.

**Summary counts (from the source file):**
- Total talkgroups: 2,102
- Prefix groups: 150
- Encryption: Secure 141; Clear 1,961
- Agency restricted: YES 986 (about 47%); NO 1,114; blank 2
- Data-quality notes: 463 rows have a blank Motorola Talk Group ID;
  3 rows have a blank display alias; 2 rows have a blank restricted
  flag. These need cleanup before any distribution.

**Organization method:** Grouped by the leading element of the talk
group name, sorted alphabetically. No region mapping has been inferred:
prefixes resembling region codes appear in the data, but they have NOT
been assigned to regions — that mapping needs SWIC confirmation.

**Control flag (important):** About 47% of the listed talkgroups are
marked agency-restricted. Under a Controlled (CUI) edition, how those
rows are handled (included as CUI, or held back) must be confirmed
before distribution. This working draft is private; it is not the
distributed edition.

---

---

## Radio Template Programming Requirements (CARRIED FORWARD FROM V3.0 — VERIFY)

**Status:** Carried forward from Version 3.0 (November 2022) as a starting draft. To be updated by the SWIC over winter 2026-27. Do not treat as current until verified. v3.0 page footers/markings have been stripped; content is otherwise verbatim.

Requirements
LICENSING DISCLAIMER

RA
FT

Nothing in this document shall be construed to serve as
authorization for any agency or individual to operate equipment
on radio channels without the proper authorization or licensing
by the Federal Communications Commission (FCC).

MINIMUM RECOMMENDED CHANNELS

The channels listed in the following tables consist of the
minimum recommended radio channels to provide for public
safety interoperable communications.

Utah Minimum Recommended VHF Channels

Table 19: VHF Programming Template - All Disciplines

MINIMUM RECOMMENDED CHANNELS – All Disciplines

CHANNEL
NAME

MOB RECV

MOB XMIT

FREQ

FREQ

A
D

NOTES

Page | 63 70 -

​

TONE

​

TONE

Utah Interoperable Communications
Field Operations Guide Ver 3.0​

November 2022

MINIMUM RECOMMENDED CHANNELS – All Disciplines
MOB RECV

MOB XMIT

A
D

NOTES

RA
FT

CHANNEL
NAME

All channels are Narrowband, Analog, Conventional

Table 20: VHF Programming Template – Law Enforcement

MINIMUM RECOMMENDED CHANNELS – Law Enforcement

CHANNEL
NAME

MOB RECV

MOB XMIT

FREQ

FREQ

TONE

TONE

A
D

NOTES

All channels are Narrowband, Analog, Conventional
Channels listed above are in addition to those listed in the ALL-DISCIPLINES programming
table

Table 21: VHF Programming Template – Fire/EMA/First Responder

MINIMUM RECOMMENDED CHANNELS – Fire/EMA/First Responder

CHANNEL
NAME

MOB RECV

MOB XMIT

FREQ

FREQ

A
D

NOTES

Page | 64 70 -

​

TONE

​

TONE

Utah Interoperable Communications
Field Operations Guide Ver 3.0​

November 2022

MINIMUM RECOMMENDED CHANNELS – Fire/EMA/First Responder
CHANNEL
NAME

MOB RECV

MOB XMIT

A
D

NOTES

RA
FT

All channels are Narrowband, Analog, Conventional
Channels listed above are in addition to those listed in the ALL-DISCIPLINES programming
table

Table 22: Programming Template - EMS

MINIMUM RECOMMENDED CHANNELS – EMS

CHANNEL
NAME

MOB RECV

MOB XMIT

FREQ

FREQ

TONE

TONE

A
D

NOTES

– VMED28 formerly known as Hospital Emergency Ambulance Radio (HEAR)

All channels are Narrowband, Analog, Conventional
Channels listed above are in addition to those listed in the ALL-DISCIPLINES programming
table

Utah Minimum Recommended UHF Channels

Table 23: UHF Programming Template - All Disciplines

MINIMUM RECOMMENDED CHANNELS – All Disciplines

CHANNEL
NAME

MOB RECV

MOB XMIT

FREQ

FREQ

A
D

NOTES

Page | 65 70 -

​

TONE

​

TONE

Utah Interoperable Communications
Field Operations Guide Ver 3.0​

November 2022

MINIMUM RECOMMENDED CHANNELS – All Disciplines
CHANNEL
NAME
UTAC43D

MOB RECV

453.8625

156.7

MOB XMIT

453.8625

A
D

156.7

NOTES
A

Incident Coordination

RA
FT

●​ Base station channel use requires an FCC license.
●​ Mobile/portable use under blanket authorization by the FCC.
●​ All channels are Narrowband, Analog, Conventional

Table 24: UHF Programming Template

MINIMUM RECOMMENDED CHANNELS – All Disciplines

CHANNEL
NAME

MOB RECV

MOB XMIT

FREQ

FREQ

A
D

NOTES

Page | 66 70 -

​

TONE

​

TONE

Utah Interoperable Communications
Field Operations Guide Ver 3.0​

November 2022

Utah Minimum Recommended 700 MHz Channels
Table 25: 700 MHz Programming Template - All Disciplines

MINIMUM RECOMMENDED CHANNELS – All Disciplines
MOB RECV

MOB XMIT

FREQ

FREQ

TONE

TONE

A
D

NOTES

RA
FT

CHANNEL
NAME

●​ Base station channel use requires an FCC license.
●​ Mobile/portable use under blanket authorization by the FCC.
●​ All channels are Narrowband, Digital P-25 Phase I Conventional
●​ Refer to FCC Region 3 700 MHz Plan for additional details and frequency listings

​

​

Page | 67 70 -

Utah Interoperable Communications
Field Operations Guide Ver 3.0​

November 2022

Utah Minimum Recommended 800 MHz Channels
Table 26: 800 MHz Programming Template - All Disciplines

MINIMUM RECOMMENDED CHANNELS – All Disciplines
MOB RECV

MOB XMIT

FREQ

FREQ

TONE

TONE

A
D

NOTES

RA
FT

CHANNEL
NAME

●​ Base station channel use requires an FCC license.
●​ Mobile/portable use under blanket authorization by the FCC.
●​ All channels are Wideband, Analog, Conventional

​

​

Page | 68 70 -

Utah Interoperable Communications
Field Operations Guide Ver 3.0​

November 2022

## What we know (filled in) vs. what still needs verification

**Filled in from known information:**
- Cover, version, authority, publisher, distribution (Controlled/CUI)
- Utah Regions section (8-region structure)
- 700 MHz section rename + organized fleet listing + summary counts
- Radio Template Programming Requirements (carried forward from v3.0, marked VERIFY — SWIC update over winter 2026-27)

**Still to verify / fill:**
- PSAP Information currency and contact details
- SWIC contact block update (v3.0 names a prior holder)
- Other 800 MHz references throughout the guide (review individually)
- Region-code prefix mapping for the talkgroup listing (confirm or
  correct; do not assume)
- Blank-field cleanup (463 missing talkgroup IDs, 3 missing aliases,
  2 missing restricted flags)
- Restricted-row handling under CUI (include as CUI vs. hold back)
- Currency of the remaining placeholder sections (repeaters, gateways,
  transportable repeaters, radio caches, data devices, templates,
  capabilities) — carried forward only after review, not assumed current

---

## Hosting note (corrected)

The empty format shell is a static file and could sit anywhere, but
this populated, controlled edition must NOT go on public GitHub Pages.
A controlled edition needs access-controlled hosting (login gate or
restricted network) before any distribution. No part of this working
draft has been published or uploaded anywhere.
