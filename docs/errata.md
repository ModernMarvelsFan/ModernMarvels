# Upstream Database Errata & Action Registry

> **Status:** Active Community Tracking Document  
> **Last Updated:** September 2, 2026  
> **Scope:** Corrections required on **TheTVDB**, **The Movie Database (TMDB)**, and **IMDb** based on primary broadcast evidence (spoken audio transcripts, on-screen credit rolls, and optical copyright cards).

This document tracks erroneous episode entries across commercial databases that corrupt automated media managers (Plex, Sonarr, Kodi). Community editors and database moderators should use the citations below to delete, merge, or correct upstream records.

---

## 🚨 Priority 1: Required Deletions (Unrelated Shows)

These entries represent **completely unrelated television programs** that were mistakenly added to the *Modern Marvels* series listing by upstream contributors. They must be permanently deleted from the series on the respective database:

| Canonical ID | Database & ID | Erroneous Listing Title | Action Required | Evidence & Rationale |
| :---: | :---: | :--- | :---: | :--- |
| `MME00731` | [TheTVDB #9277357](https://thetvdb.com/series/modern-marvels/episodes/9277357) | **World's Largest Cricket Stadium** | 🔴 **DELETE** | Completely unrelated television production. This program was produced and broadcast exclusively in India by regional network History TV18 as a standalone special titled 'Modern Marvel: World's Largest Cricket Stadium' (singular 'Marvel'), detailing the construction of the Narendra Modi Stadium in Ahmedabad. It was not produced by or affiliated with Actuality Productions / A+E Networks for the US series Modern Marvels. It must be permanently removed from the TheTVDB Modern Marvels episode list. |
| `MME00171` | [TheTVDB #10579417](https://thetvdb.com/series/modern-marvels/episodes/10579417) | **How Did They Build That?: Concrete** | 🔴 **DELETE** | Completely separate architectural documentary series. 'How Did They Build That?' is an independent British / Smithsonian Channel television series produced by Curve Media. An upstream contributor erroneously cataloged this episode under TheTVDB Modern Marvels Season 8. It bears zero production connection to Modern Marvels and must be deleted from the series listing. |
| `MME00754` | Canonical Pipeline | **None (Corrupted Placeholder)** | 🔴 **PURGE** | Empty placeholder slot containing null title, 0 files, and no upstream database IDs. Purged from canonical tracking. |
| `MME00755` | Canonical Pipeline | **None (Corrupted Placeholder)** | 🔴 **PURGE** | Empty placeholder slot containing null title, 0 files, and no upstream database IDs. Purged from canonical tracking. |

---

## ✂️ Priority 2: Required Splits (Conflated Episodes)

These entries merged two distinct standalone 1-hour broadcast episodes into a single 2-hour entry:

| Canonical ID | Database & ID | Conflated Listing Title | Action Required | Evidence & Rationale |
| :---: | :---: | :--- | :---: | :--- |
| `MME00208 / MME00225` | [TMDB #1023188 (S09E04)](https://www.themoviedb.org/tv/6145-modern-marvels/season/9/episode/4) | **Big Rigs of Combat: Tanks and Jeeps** | 🟡 **SPLIT** | TMDB merged two completely distinct 1-hour broadcast documentaries into a single 2-hour record under S09E04 ('Tanks and Jeeps'). Primary broadcast audio, spoken title cards, and TheTVDB verify they were produced and aired as two standalone episodes: (1) 'Big Rigs of Combat: Tanks' (MME00208; TheTVDB #296761) and (2) 'Big Rigs of Combat: Jeeps' (MME00225; TheTVDB #9262279). TMDB must split S09E04 into two distinct consecutive episode numbers. |

---

## 🔄 Priority 3: Required Merges & Duplicate Purges

Entries that duplicate an existing canonical episode due to rerun air dates or '(2)' suffix additions:

| Canonical ID | Database & ID | Listing Title | Action Required | Evidence & Rationale |
| :---: | :---: | :--- | :---: | :--- |
| `MME00750` | [TheTVDB #11755189](https://thetvdb.com/series/modern-marvels/episodes/11755189) | **The Sears Tower** | 🟠 **DELETE / MERGE** | Erroneous submission listing an air date of October 13, 2024. Original series production concluded by 2022. This is a duplicate rerun entry of the canonical 2004 documentary 'The Sears Tower' (MME00395; TMDB S11E39, TheTVDB #320448, IMDb tt1055722). TheTVDB record #11755189 must be deleted as a duplicate. |
| `MME00458` | [TheTVDB #7930503](https://thetvdb.com/series/modern-marvels/episodes/7930503) | **The Golden Gate Bridge (2)** | 🟠 **DELETE / MERGE** | Upstream contributor created a duplicate entry appending '(2)' for a May 2005 rebroadcast. The program is the canonical 1995 documentary 'The Golden Gate Bridge' (MME00017; TheTVDB #320422). Must be merged into #320422. |
| `MME00519` | [TheTVDB #7930575](https://thetvdb.com/series/modern-marvels/episodes/7930575) | **The Telephone (2)** | 🟠 **DELETE / MERGE** | Upstream contributor created a duplicate entry appending '(2)' for a May 2006 rebroadcast. The program is the canonical 1996 documentary 'The Telephone' (MME00032; TheTVDB #320448). Must be merged into #320448. |
| `MME00707` | [TheTVDB #11750141](https://thetvdb.com/series/modern-marvels/episodes/11750141) | **Engines** | 🟠 **DELETE / MERGE** | Created on TheTVDB with a 2012 air date. This duplicates the canonical 2002 documentary 'Engines' (MME00220; TheTVDB #296758, TMDB S09E16). Must be deleted. |
| `MME00089 / MME00258` | [TheTVDB / TMDB #TheTVDB #11742239 vs TMDB #1023237](https://thetvdb.com/series/modern-marvels/episodes/11742239) | **Garbage** | 🟠 **CONSOLIDATE** | TheTVDB and TMDB created two disconnected listings for the same documentary with divergent air dates. On-screen copyright cards date the production to 1999; TMDB's 2002 date represents a syndication rebroadcast. |
| `MME00159 / MME00333` | [TheTVDB / TMDB #TheTVDB #1335471 vs TMDB #1023248](https://thetvdb.com/series/modern-marvels/episodes/1335471) | **U-Boats** | 🟠 **CONSOLIDATE** | TheTVDB and TMDB have divergent listings. Broadcast audio and copyright cards confirm the production aired originally in 2001. TMDB's S10E64 entry is a syndication package of the same film. |
| `MME00204 / MME00350` | [TheTVDB / TMDB #TheTVDB #11749934 vs TMDB #1023184](https://thetvdb.com/series/modern-marvels/episodes/11749934) | **Failed Inventions** | 🟠 **CONSOLIDATE** | Duplicate entries representing the same documentary. Original broadcast occurred in January 2002; TheTVDB record #11749934 is a late duplicate. |

---

## 📅 Priority 4: Severe Air Date Divergences (≥ 4 Years)

Episodes where TheTVDB and TMDB diverge by four or more years due to rerun confusion or misattributed production windows:

| Canonical ID | Episode Title | TMDB Air Date | TheTVDB Air Date | Divergence | Primary Evidence Finding |
| :---: | :--- | :---: | :---: | :---: | :--- |
| `MME00006` | **Transatlantic Cable** | `1994-03-27` | `1998-08-17` | **4 years** | Copyright © 1994 A&E. TMDB holds the correct original broadcast air date. TheTVDB listing represents a 1998 repeat. |
| `MME00007` | **Balloons** | `1994-12-16` | `1999-12-16` | **5 years** | Copyright © 1994. TheTVDB incorrectly indexed this under December 1999. |
| `MME00023` | **The NYC Subway** | `1995-10-19` | `1999-01-06` | **4 years** | Copyright © 1995. TMDB date corroborated by historical TV Guide listings from October 1995. |
| `MME00107` | **More Earthmovers** | `1999-10-18` | `2006-10-09` | **7 years** | Copyright © 1999. TheTVDB logged an October 2006 rerun date. |
| `MME00402` | **Firefighting: The Arson Detectives** | `2004-09-30` | `1998-11-17` | **6 years** | TheTVDB conflated this 2004 production with an earlier 1998 firefighting documentary. |
| `MME00443` | **Firefighting!: Extreme Conditions** | `2005-02-15` | `1998-12-08` | **7 years** | TheTVDB applied the 1998 broadcast date of 'Firefighting! Containing the Demon' to this 2005 production. |
| `MME00544` | **Shotguns** | `2006-09-17` | `1999-05-23` | **7 years** | On-screen graphics and copyright cards date this high-definition production to 2006. TheTVDB 1999 date is erroneous. |
| `MME00668` | **Helicopters** | `2010-04-29` | `1998-09-14` | **12 years** | Modern Marvels produced two distinct documentaries titled 'Helicopters' (1998 and 2010). TheTVDB mapped both to 1998. |

---

## How to Submit Upstream Corrections

When submitting tickets to database moderators:
1. **TheTVDB:** Post a ticket at [support.thetvdb.com](https://support.thetvdb.com) referencing the specific Episode ID and citing the primary copyright year and dialogue transcript URL from this archive.
2. **TMDB:** Post a content report on the specific episode's discussion forum referencing the standalone 1-hour broadcast recordings.
3. **Link to Evidence:** Always provide the direct URL to the episode's dossier in this archive (`https://shanto.github.io/Modern-Marvels-Public/episodes/MME#####/`) as the primary proof.
