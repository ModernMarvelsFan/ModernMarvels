# Upstream Database Errata & Action Registry

> **Status:** Active Community Tracking Document  
> **Last Updated:** September 2, 2026  
> **Scope:** Systematic corrections required on **TheTVDB**, **The Movie Database (TMDB)**, and **IMDb** based on primary broadcast evidence (spoken audio transcripts, on-screen credit rolls, optical copyright cards, and internal temporal references).

This document tracks erroneous episode entries across commercial databases that corrupt automated media managers (Plex, Sonarr, Kodi). Community editors and database moderators should use the citations below to delete, merge, or correct upstream records.

---

## 💡 Methodology: Copyright Cards vs. Premiere Releases vs. Re-Edits

When analyzing historical documentaries, **an on-screen copyright year does not always equal the original broadcast premiere date**:
* **Syndication & Series Re-branding:** The History Channel routinely re-packaged documentaries from sister series (such as Greystone Communications' *Tales of the Gun*) under the *Modern Marvels* banner years later. For example, *Shotguns* carried an on-screen title of *Tales of the Gun* with a `© MCMXCIX (1999)` copyright card, yet TMDB cataloged it as a 2006 Modern Marvels episode (`S13E38`).
* **Updated & Revised Cuts:** Popular episodes were updated with newer footage years after their premiere. For instance, *More Earthmovers* carried a `© 1999` copyright, but later broadcasts burned a `© 2005` copyright and inserted dialogue discussing **Hurricane Katrina (August 2005)**.
* **Internal Transcript Temporal Forensics:** Rather than trusting commercial catalog dates or standalone copyright years, this archive examines **spoken dialogue references** (e.g., whether an event like Katrina is spoken of as past history, or whether an aerospace mission in 2003 is described as a future plan).

---

## 🚨 Priority 1: Required Deletions (Unrelated Shows)

These entries represent **completely unrelated television programs** that were mistakenly added to the *Modern Marvels* series listing by upstream contributors. They must be permanently deleted from the series on the respective database:

| Episode ID | Database & ID | Erroneous Listing Title | Action Required | Evidence & Rationale |
| :---: | :---: | :--- | :---: | :--- |
| [`MME00731`](episodes/MME00731.md) | [TheTVDB #9277357](https://thetvdb.com/series/modern-marvels/episodes/9277357) | **World's Largest Cricket Stadium** | 🔴 **DELETE** | Completely unrelated television production. This program was produced and broadcast exclusively in India by regional network History TV18 as a standalone special titled 'Modern Marvel: World's Largest Cricket Stadium' (singular 'Marvel'), detailing the construction of the Narendra Modi Stadium in Ahmedabad. It was not produced by or affiliated with Actuality Productions / A+E Networks for the US series Modern Marvels. It must be permanently removed from the TheTVDB Modern Marvels episode list. |
| [`MME00171`](episodes/MME00171.md) | [TheTVDB #10579417](https://thetvdb.com/series/modern-marvels/episodes/10579417) | **How Did They Build That?: Concrete** | 🔴 **DELETE** | Completely separate architectural documentary series. 'How Did They Build That?' is an independent British / Smithsonian Channel television series produced by Curve Media. An upstream contributor erroneously cataloged this episode under TheTVDB Modern Marvels Season 8. It bears zero production connection to Modern Marvels and must be deleted from the series listing. |
| [`MME00754`](episodes/MME00754.md) | Internal Pipeline | **None (Corrupted Placeholder)** | 🔴 **PURGE** | Empty placeholder slot containing null title, 0 files, and no upstream database IDs. Purged from episode tracking. |
| [`MME00755`](episodes/MME00755.md) | Internal Pipeline | **None (Corrupted Placeholder)** | 🔴 **PURGE** | Empty placeholder slot containing null title, 0 files, and no upstream database IDs. Purged from episode tracking. |

---

## ✂️ Priority 2: Required Splits (Conflated Episodes)

These entries merged two distinct standalone 1-hour broadcast episodes into a single 2-hour entry:

| Episode ID | Database & ID | Conflated Listing Title | Action Required | Evidence & Rationale |
| :---: | :---: | :--- | :---: | :--- |
| [`MME00208`](episodes/MME00208.md) / [`MME00225`](episodes/MME00225.md) | [TMDB #1023188 (S09E04)](https://www.themoviedb.org/tv/6145-modern-marvels/season/9/episode/4) | **Big Rigs of Combat: Tanks and Jeeps** | 🟡 **SPLIT** | TMDB merged two completely distinct 1-hour broadcast documentaries into a single 2-hour record under S09E04 ('Tanks and Jeeps'). Primary broadcast audio, spoken title cards, and TheTVDB verify they were produced and aired as two standalone episodes: (1) 'Big Rigs of Combat: Tanks' (MME00208; TheTVDB #296761) and (2) 'Big Rigs of Combat: Jeeps' (MME00225; TheTVDB #9262279). TMDB must split S09E04 into two distinct consecutive episode numbers. |

---

## 🔄 Priority 3: Required Merges & Duplicate Purges

Entries that duplicate an existing master episode due to rerun air dates or '(2)' suffix additions:

| Episode ID | Database & ID | Listing Title | Action Required | Evidence & Rationale |
| :---: | :---: | :--- | :---: | :--- |
| [`MME00750`](episodes/MME00750.md) | [TheTVDB #11755189](https://thetvdb.com/series/modern-marvels/episodes/11755189) | **The Sears Tower** | 🟠 **DELETE / MERGE** | Erroneous submission listing an air date of October 13, 2024. Original series production concluded by 2022. This is a duplicate rerun entry of the original 2004 documentary 'The Sears Tower' (MME00395; TMDB S11E39, TheTVDB #320448, IMDb tt1055722). TheTVDB record #11755189 must be deleted as a duplicate. |
| [`MME00458`](episodes/MME00458.md) | [TheTVDB #7930503](https://thetvdb.com/series/modern-marvels/episodes/7930503) | **The Golden Gate Bridge (2)** | 🟠 **DELETE / MERGE** | Upstream contributor created a duplicate entry appending '(2)' for a May 2005 rebroadcast. The program is the original 1995 documentary 'The Golden Gate Bridge' (MME00017; TheTVDB #320422). Must be merged into #320422. |
| [`MME00519`](episodes/MME00519.md) | [TheTVDB #7930575](https://thetvdb.com/series/modern-marvels/episodes/7930575) | **The Telephone (2)** | 🟠 **DELETE / MERGE** | Upstream contributor created a duplicate entry appending '(2)' for a May 2006 rebroadcast. The program is the original 1996 documentary 'The Telephone' (MME00032; TheTVDB #320448). Must be merged into #320448. |
| [`MME00707`](episodes/MME00707.md) | [TheTVDB #11750141](https://thetvdb.com/series/modern-marvels/episodes/11750141) | **Engines** | 🟠 **DELETE / MERGE** | Created on TheTVDB with a 2012 air date. This duplicates the original 2002 documentary 'Engines' (MME00220; TheTVDB #296758, TMDB S09E16). Must be deleted. |
| [`MME00089`](episodes/MME00089.md) / [`MME00258`](episodes/MME00258.md) | [TheTVDB / TMDB #TheTVDB #11742239 vs TMDB #1023237](https://thetvdb.com/series/modern-marvels/episodes/11742239) | **Garbage** | 🟠 **CONSOLIDATE** | TheTVDB and TMDB created two disconnected listings for the same documentary with divergent air dates. On-screen copyright cards date the production to 1999; TMDB's 2002 date represents a syndication rebroadcast. |
| [`MME00159`](episodes/MME00159.md) / [`MME00333`](episodes/MME00333.md) | [TheTVDB / TMDB #TheTVDB #1335471 vs TMDB #1023248](https://thetvdb.com/series/modern-marvels/episodes/1335471) | **U-Boats** | 🟠 **CONSOLIDATE** | TheTVDB and TMDB have divergent listings. Broadcast audio and copyright cards confirm the production aired originally in 2001. TMDB's S10E64 entry is a syndication package of the same film. |
| [`MME00204`](episodes/MME00204.md) / [`MME00350`](episodes/MME00350.md) | [TheTVDB / TMDB #TheTVDB #11749934 vs TMDB #1023184](https://thetvdb.com/series/modern-marvels/episodes/11749934) | **Failed Inventions** | 🟠 **CONSOLIDATE** | Duplicate entries representing the same documentary. Original broadcast occurred in January 2002; TheTVDB record #11749934 is a late duplicate. |

---

## 📅 Priority 4: Air Date Divergences & Forensic Transcript Analysis

Episodes where TheTVDB and TMDB diverge significantly, resolved via optical copyright cards and transcript temporal markers:

| Episode ID | Episode Title | TMDB Date | TheTVDB Date | Forensic Verdict | Primary Evidence Finding |
| :---: | :--- | :---: | :---: | :--- | :--- |
| [`MME00544`](episodes/MME00544.md) | **Shotguns** | `2006-09-17` | `1999-05-23` | **Original 1999 production, re-packaged under Modern Marvels in 2006** | Primary optical credits prove this film was produced by Greystone Communications, Inc. under the on-screen title 'Tales of the Gun' with copyright '© MCMXCIX (1999) A&E Television Networks'. TheTVDB (1999-05-23) and IMDb (1999) record the genuine original premiere date. TMDB (2006-09-17, S13E38) records a syndication rebroadcast when The History Channel re-packaged several Greystone gun documentaries under the Modern Marvels umbrella. The copyright and production personnel confirm a 1999 origin, not 2006. |
| [`MME00107`](episodes/MME00107.md) | **More Earthmovers** | `1999-10-18` | `2006-10-09` | **Revised 2006 cut incorporating post-2005 footage** | Optical copyright cards on the broadcast master carry dual years: '© 1999, 2005 Actuality Productions'. Crucially, transcript analysis reveals explicit dialogue referencing Hurricane Katrina: 'Hurricane Katrina made landfall in Mississippi on 29 August 2005...'. Because Katrina occurred in August 2005, the broadcast version cannot be the 1999 original. TheTVDB's air date of October 9, 2006 accurately dates this revised broadcast. |
| [`MME00243`](episodes/MME00243.md) | **Jet Engines** | `2002-08-21` | `1999-05-03` | **Original 1999 production; TMDB reflects repeat** | Optical copyright card reads '© 1999 Actuality Productions'. Transcript internal dating confirms 1999 as the contemporary baseline: the narrator remarks 'no one would ever have anticipated that the airplane would have been flying in 1999, or as it probably will be in 2019' (treating 1999 as present and 2019 as future). TheTVDB's 1999-05-03 date is the verified original premiere. |
| [`MME00668`](episodes/MME00668.md) | **Helicopters** | `2010-04-29` | `1998-09-14` | **Completely different 2010 HD documentary conflated with 1998 classic** | Optical copyright card reads '© 2009 Actuality Productions, Inc.'. Dialogue references 2008 production milestones: 'produce nearly 900 helicopters in 2008... winning Popular Science's Best of What's New award in 2008'. TheTVDB's 1998 date is an erroneous mapping to an earlier 1998 episode of the same name. TMDB's 2010-04-29 air date is correct. |
| [`MME00007`](episodes/MME00007.md) | **Balloons** | `1994-12-16` | `1999-12-16` | **1999 production; TMDB date is erroneous** | Transcript dialogue discusses NASA exploration milestones scheduled for the future: 'NASA plans to launch its first interplanetary aerobot by rocket in 2003... scheduled to enter the atmosphere of Venus and Titan in 2005'. These plans were formulated in the late 1990s, refuting TMDB's 1994 date and confirming TheTVDB's December 1999 broadcast. |
| [`MME00573`](episodes/MME00573.md) | **More Ice** | `2007-02-11` | `2009-10-28` | **2007 premiere; TheTVDB date is a late repeat** | Optical copyright card reads '© 2007 History Television Network Productions'. Transcript references research expeditions conducted in 2006: 'in 2006, scientists from California's Monterey Bay Aquarium Research Institute sailed to the Pacific coastal waters'. Corroborates TMDB's February 11, 2007 air date; TheTVDB's 2009 date is a syndicated repeat. |

---

## How to Submit Upstream Corrections

When submitting tickets to database moderators:
1. **TheTVDB:** Post a ticket at [support.thetvdb.com](https://support.thetvdb.com) referencing the specific Episode ID and citing the primary copyright year, dialogue transcript URL, and temporal evidence from this archive.
2. **TMDB:** Post a content report on the specific episode's discussion forum referencing the standalone 1-hour broadcast recordings.
3. **Link to Evidence:** Always provide the direct URL to the episode's dossier in this archive (`https://modernmarvelsfan.github.io/ModernMarvels/episodes/MME#####/`) as the primary proof.
