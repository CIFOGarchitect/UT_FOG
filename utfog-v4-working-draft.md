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
updated by the SWIC over winter 2026-27), National Interoperability Channels (NIFOG) (CISA public source). All other sections
from the v3.0 table of contents remain placeholders pending content
review: Establishing Interoperability, Introduction, State Maps,
Interoperability and Incident Management, Communications Unit (COMU),
Requests for Communications Assets, Federal Interoperability Channel Plan, PSAP Information, Nationwide Interop Channel
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

### Talkgroup governance and stewardship

**Source:** Statewide Talkgroup Governance & Interoperability Stewardship Program (SWIC office), incorporated per SWIC direction, Oct 24, 2026.

**Status note:** The SCIP is currently under update with CISA technical assistance, and the BRAG TICP update is targeted by end of year 2026. Alignment references in this section should be refreshed when those updates land.

**Roles.** UCA System Administration owns network infrastructure: network health, microwave backhaul, tower sites, core routing, system capacity, RF performance, and hardware maintenance. The SWIC office owns talkgroup policy and governance: operational stewardship, agency access criteria, Statewide Communication Plan (SCIP) alignment, regional TICP templates, codeplug standardization, and mutual-aid talkgroup allocation. The separation lets engineering focus on core performance while assignments reflect the statewide operational interop strategy.

**Authorization and gatekeeping.** The SWIC office is the review and approval authority for all local, regional, and statewide talkgroup allocation and modification requests. Requests use a standardized form covering operational need, subscriber counts, coverage footprint, and talkgroup longevity. Criteria distinguish local single-site talkgroups from wide-area roaming talkgroups, preventing talkgroup sprawl and protecting core capacity and site loading.

**SCIP and TICP alignment.** All provisioning aligns with the Statewide Communication Plan and the regional Tactical Interoperability Communications Plans. The SWIC office maintains the standardized statewide interop zone templates across the eight Emergency Management Regions (per the region map).

**Tactical and event management.** The SWIC office oversees allocation, reservation, and real-time management of statewide and regional event talkgroups during major multi-jurisdictional incidents, wildland fires, or planned events, including rules for console-to-console patching, radio-to-radio patching, and inter-system gateways to prevent audio feedback loops and system congestion.

**Master directory stewardship and auditing.** The Utah Master Talkgroup Directory is the single authoritative source of truth for talkgroup assignments statewide. Periodic utilization audits, alongside UCA system performance reports, identify dormant or inactive talkgroups for decommissioning.

**Provisioning workflow (5 steps).**
1. Request submission — the requesting agency submits the standardized form.
2. Operational review — the SWIC office audits the request against SCIP/TICP standards, naming conventions, and encryption rules, and approves, modifies, or denies it.
3. Technical review — UCA engineering reviews the approved request for core capacity, bandwidth impact, site licensing, and system ID availability.
4. Core provisioning — UCA provisions the approved talkgroup in the P25 core.
5. Documentation — the SWIC office logs the assignment in the Master Talkgroup Directory and notifies the agency.

Codeplug standardization, naming conventions, and encryption strapping policy are covered under Radio Template Programming Requirements.

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

---

## National Interoperability Channels (NIFOG) (POPULATED — CISA PUBLIC SOURCE — Oct 24, 2026)

**Source:** CISA, National Interoperability Field Operations Guide (NIFOG) v2.01 (public). Channel names follow the ANSI/APCO/NPSTC standard channel nomenclature. This section covers the non-federal national interoperability channels. Federal Incident Response (IR) and Law Enforcement (LE) channels are in the full NIFOG; as a convention, analog federal channels transmit CTCSS 167.9 Hz with carrier squelch receive, and P25 federal channels use NAC $68F.

**Conventions.** A "D" suffix means direct (simplex) operation on the repeater output frequency. Calling channels are for initial contact — move to a tactical channel after contact. Use requires proper FCC authorization/licensing (see cover licensing note).

### VHF — simplex

Tone 156.7 Hz CTCSS on all channels below.

| Channel | Receive (MHz) | Transmit (MHz) | Use |
|---|---|---|---|
| VCALL10 | 155.7525 | Simplex | Calling |
| VTAC11 | 151.1375 | Simplex | Tactical |
| VTAC12 | 154.4525 | Simplex | Tactical |
| VTAC13 | 158.7375 | Simplex | Tactical |
| VTAC14 | 159.4725 | Simplex | Tactical |
| VFIRE21 | 154.2800 | Simplex | Fire |
| VFIRE22 | 154.2650 | Simplex | Fire |
| VFIRE23 | 154.2950 | Simplex | Fire |
| VFIRE24 | 154.2725 | Simplex | Fire |
| VFIRE25 | 154.2875 | Simplex | Fire |
| VFIRE26 | 154.3025 | Simplex | Fire |
| VMED28 | 155.3400 | Simplex | EMS |
| VMED29 | 155.3475 | Simplex | EMS |
| VLAW31 | 155.4750 | Simplex | Law enforcement |
| VLAW32 | 155.4825 | Simplex | Law enforcement |

### VHF — repeater pairs

Tone 156.7 Hz CTCSS.

| Channel | Receive (MHz) | Transmit (MHz) | Use |
|---|---|---|---|
| VTAC17 | 161.8500 | 157.2500 | Tactical repeater (limited to 33 inland areas) |
| VTAC17D | 161.8500 | Simplex | Tactical direct (limited to 33 inland areas) |
| VTAC33 | 159.4725 | 151.1375 | Tactical repeater |
| VTAC34 | 158.7375 | 154.4525 | Tactical repeater |
| VTAC35 | 159.4725 | 158.7375 | Tactical repeater |
| VTAC36 | 151.1375 | 159.4725 | Tactical repeater |
| VTAC37 | 154.4525 | 158.7375 | Tactical repeater |
| VTAC38 | 158.7375 | 159.4725 | Tactical repeater |

### VHF low band

Tone 156.7 Hz CTCSS.

| Channel | Receive (MHz) | Transmit (MHz) | Use |
|---|---|---|---|
| LLAW1 | 39.4600 | 45.8600 | Law enforcement |
| LFIRE2 | 39.4800 | 45.8800 | Fire |
| LLAW3 | 45.8600 | 39.4600 | Law enforcement |
| LFIRE4 | 45.8800 | 39.4800 | Fire |

### UHF

Tone 156.7 Hz CTCSS, narrowband FM. Each channel below also has a D direct variant on the output frequency.

| Channel | Receive (MHz) | Transmit (MHz) | Use |
|---|---|---|---|
| UCALL40 | 453.2125 | 458.2125 | Calling |
| UTAC41 | 453.4625 | 458.4625 | Tactical |
| UTAC42 | 453.7125 | 458.7125 | Tactical |
| UTAC43 | 453.8625 | 458.8625 | Tactical |

### 700 MHz

P25 digital only, NAC $293; analog operation is not permitted. Each repeater channel below also has a D direct variant on the output frequency.

| Channel | Receive (MHz) | Transmit (MHz) | Use |
|---|---|---|---|
| 7CALL50 | 769.24375 | 799.24375 | Primary calling |
| 7TAC51 | 769.14375 | 799.14375 | General public safety |
| 7TAC52 | 769.64375 | 799.64375 | General public safety |
| 7TAC53 | 770.14375 | 800.14375 | General public safety |
| 7TAC54 | 770.64375 | 800.64375 | General public safety |
| 7TAC55 | 769.74375 | 799.74375 | General public safety |
| 7TAC56 | 770.24375 | 800.24375 | General public safety |
| 7GTAC57 | 770.99375 | 800.99375 | Other public service |
| 7MOB59 | 770.89375 | 800.89375 | Mobile repeater |
| 7LAW61 | 770.39375 | 800.39375 | Law enforcement |
| 7LAW62 | 770.49375 | 800.49375 | Law enforcement |
| 7FIRE63 | 769.89375 | 799.89375 | Fire |
| 7FIRE64 | 769.99375 | 799.99375 | Fire |
| 7MED65 | 769.39375 | 799.39375 | EMS |
| 7MED66 | 769.49375 | 799.49375 | EMS |
| 7DATA69 | 770.74375 | 800.74375 | Mobile data |
| 7CALL70 | 773.25625 | 803.25625 | Secondary calling |
| 7TAC71 | 773.10625 | 803.10625 | General public safety |

Note: NIFOG lists additional 700 MHz channels (7TAC72–76, 7GTAC77, 7MOB79, 7LAW81–82, 7FIRE83–84, 7MED86–87, 7DATA89) — see the full NIFOG for those.

### 800 MHz

Tone 156.7 Hz CTCSS. Each channel below also has a D direct variant on the output frequency.

| Channel | Receive (MHz) | Transmit (MHz) | Use |
|---|---|---|---|
| 8CALL90 | 851.0125 | 806.0125 | Calling |
| 8TAC91 | 851.5125 | 806.5125 | Tactical |
| 8TAC92 | 852.0125 | 807.0125 | Tactical |
| 8TAC93 | 852.5125 | 807.5125 | Tactical |
| 8TAC94 | 853.0125 | 808.0125 | Tactical |

**Full reference.** The complete NIFOG (v2.01) is available free from CISA's SAFECOM field operations guides page and as the eNIFOG mobile app (works offline).

## What we know (filled in) vs. what still needs verification

**Filled in from known information:**
- Cover, version, authority, publisher, distribution (Controlled/CUI)
- Utah Regions section (8-region structure)
- 700 MHz section rename + organized fleet listing + summary counts
- 700 MHz talkgroup governance and stewardship (from the governance program, per SWIC direction Oct 24)
- National Interoperability Channels (NIFOG) (CISA NIFOG v2.01, public source)
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
