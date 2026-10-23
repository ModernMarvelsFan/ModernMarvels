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
| [`MME00208`](episodes/MME00208.md) / [`MME00225`](episodes/MME00225.md) | [TMDB #1023188 (S09E04)](https://www.themoviedb.org/tv/6145-modern-marvels/season/9/episode/4)<br>[TheTVDB #296761](https://thetvdb.com/series/modern-marvels/episodes/296761) / [#9262279](https://thetvdb.com/series/modern-marvels/episodes/9262279) | **Big Rigs of Combat: Tanks and Jeeps** | 🟡 **SPLIT** | TMDB merged two completely distinct 1-hour broadcast documentaries into a single 2-hour record under S09E04 ('Tanks and Jeeps'). Primary broadcast audio, spoken title cards, and TheTVDB verify they were produced and aired as two standalone episodes: (1) 'Big Rigs of Combat: Tanks' ([MME00208](episodes/MME00208.md); [TheTVDB #296761](https://thetvdb.com/series/modern-marvels/episodes/296761)) and (2) 'Big Rigs of Combat: Jeeps' ([MME00225](episodes/MME00225.md); [TheTVDB #9262279](https://thetvdb.com/series/modern-marvels/episodes/9262279)). TMDB must split S09E04 into two distinct consecutive episode numbers. |

---

## 🔄 Priority 3: Duplicate Entries & Cross-Database Desynchronizations

This section addresses two distinct database problems:
1. **Internal Duplicates (within TheTVDB or TMDB):** A single database created two or more records for the same documentary (often due to syndication reruns, re-cuts, or appending `(2)`). Upstream moderators must **delete or merge** the duplicate into the primary record.
2. **Cross-Database Desynchronizations:** TheTVDB and TMDB have completely different air dates and season numbers for the same documentary. Because neither database recognized the other's listing, automated scrapers (and initial ingest pipelines) created separate "split" slots. We **consolidate** them into a single primary master episode in this archive and provide citations for upstream databases to harmonize their metadata.

---

### 3A. TheTVDB Internal Duplicates (Duplicate Records on TheTVDB)

These entries represent duplicate records created inside **TheTVDB** itself. Upstream moderators on TheTVDB should merge or delete the secondary record into the primary entry:

| Episode ID | Primary TVDB Entry (Keep) | Duplicate TVDB Entry (Delete / Merge) | Title as Listed | Action for TheTVDB | Evidence & Provenance |
| :---: | :---: | :---: | :--- | :---: | :--- |
| [`MME00395`](episodes/MME00395.md) / [`MME00750`](episodes/MME00750.md) | [TheTVDB #320448 (S11E39)](https://thetvdb.com/series/modern-marvels/episodes/320448) | [TheTVDB #11755189 (S11E44)](https://thetvdb.com/series/modern-marvels/episodes/11755189) | **The Sears Tower** | 🔴 **DELETE #11755189** | Erroneous submission listing an air date of October 13, 2024. Series production concluded in 2022. This duplicates the original 2004 broadcast ([#320448](https://thetvdb.com/series/modern-marvels/episodes/320448); [TMDB S11E39](https://www.themoviedb.org/tv/6145-modern-marvels/season/11/episode/39)). |
| [`MME00017`](episodes/MME00017.md) / [`MME00458`](episodes/MME00458.md) | [TheTVDB #296601 (S02E09)](https://thetvdb.com/series/modern-marvels/episodes/296601) | [TheTVDB #7930503 (S00E109)](https://thetvdb.com/series/modern-marvels/episodes/7930503) | **The Golden Gate Bridge (2)** | 🔴 **MERGE #7930503** | Upstream contributor appended '(2)' for a May 2005 rebroadcast. The program is identical to the original 1995 documentary ([#296601](https://thetvdb.com/series/modern-marvels/episodes/296601)). |
| [`MME00032`](episodes/MME00032.md) / [`MME00519`](episodes/MME00519.md) | [TheTVDB #303324 (S03E09)](https://thetvdb.com/series/modern-marvels/episodes/303324) | [TheTVDB #7930575 (S00E110)](https://thetvdb.com/series/modern-marvels/episodes/7930575) | **The Telephone (2)** | 🔴 **MERGE #7930575** | Upstream contributor appended '(2)' for a May 2006 rebroadcast. The program is identical to the original 1996 documentary ([#303324](https://thetvdb.com/series/modern-marvels/episodes/303324)). |
| [`MME00220`](episodes/MME00220.md) / [`MME00707`](episodes/MME00707.md) | [TheTVDB #296771 (S09E31)](https://thetvdb.com/series/modern-marvels/episodes/296771) | [TheTVDB #11750141 (S00E115)](https://thetvdb.com/series/modern-marvels/episodes/11750141) | **Engines** | 🔴 **DELETE #11750141** | Duplicate created with a 2012 rerun air date. Duplicates the original 2002 broadcast ([#296771](https://thetvdb.com/series/modern-marvels/episodes/296771); [TMDB S09E16](https://www.themoviedb.org/tv/6145-modern-marvels/season/9/episode/16)). |
| [`MME00204`](episodes/MME00204.md) / [`MME00350`](episodes/MME00350.md) | [TheTVDB #11749825](https://thetvdb.com/series/modern-marvels/episodes/11749825) | [TheTVDB #11749934 (S10E67)](https://thetvdb.com/series/modern-marvels/episodes/11749934) | **Failed Inventions** | 🔴 **MERGE #11749934** | Original broadcast occurred January 2, 2002 ([#11749825](https://thetvdb.com/series/modern-marvels/episodes/11749825)). Record #11749934 is a duplicate created from a December 2003 rerun. |
| [`MME00110`](episodes/MME00110.md) / [`MME00265`](episodes/MME00265.md) | [TheTVDB #296647 (S06E31)](https://thetvdb.com/series/modern-marvels/episodes/296647) | [TheTVDB #11749878](https://thetvdb.com/series/modern-marvels/episodes/11749878) | **Motorcycles** | 🔴 **DELETE #11749878** | Original broadcast aired November 15, 1999 ([#296647](https://thetvdb.com/series/modern-marvels/episodes/296647)). Entry #11749878 is an isolated repeat listing from December 2002. |
| [`MME00112`](episodes/MME00112.md) / [`MME00302`](episodes/MME00302.md) | [TheTVDB #296818 (S06E34)](https://thetvdb.com/series/modern-marvels/episodes/296818) | [TheTVDB #11749898](https://thetvdb.com/series/modern-marvels/episodes/11749898) | **More Engineering Disasters** | 🔴 **DELETE #11749898** | Original broadcast aired November 29, 1999 ([#296818](https://thetvdb.com/series/modern-marvels/episodes/296818)). Entry #11749898 is a rerun listing logged under 2003. |
| [`MME00120`](episodes/MME00120.md) / [`MME00279`](episodes/MME00279.md) | [TheTVDB #296655 (S07E04)](https://thetvdb.com/series/modern-marvels/episodes/296655) | [TheTVDB #11749886](https://thetvdb.com/series/modern-marvels/episodes/11749886) | **Space Stations** | 🔴 **DELETE #11749886** | Original broadcast aired February 3, 2000 ([#296655](https://thetvdb.com/series/modern-marvels/episodes/296655)). Entry #11749886 is a rerun listing logged under 2003. |
| [`MME00146`](episodes/MME00146.md) / [`MME00550`](episodes/MME00550.md) | [TheTVDB #296684 (S07E34)](https://thetvdb.com/series/modern-marvels/episodes/296684) | [TheTVDB #11750157](https://thetvdb.com/series/modern-marvels/episodes/11750157) | **Assembly Lines** | 🔴 **DELETE #11750157** | Original broadcast aired October 19, 2000 ([#296684](https://thetvdb.com/series/modern-marvels/episodes/296684)). Entry #11750157 is a repeat listing logged under 2006. |
| [`MME00083`](episodes/MME00083.md) / [`MME00167`](episodes/MME00167.md) | [TheTVDB #296621 (S06E01)](https://thetvdb.com/series/modern-marvels/episodes/296621) | [TheTVDB #9281904](https://thetvdb.com/series/modern-marvels/episodes/9281904) | **Airships** (*Then And Now: Airships*) | 🔴 **MERGE #9281904** | Repackaged syndication recut from 2001. Anchored to original 1999 production ([#296621](https://thetvdb.com/series/modern-marvels/episodes/296621)). |

---

### 3B. TMDB Internal Duplicates (Duplicate Records on TMDB)

These entries represent duplicate records created inside **The Movie Database (TMDB)** where rebroadcast dates were logged as new episodes. Upstream TMDB contributors should delete the duplicate entries:

| Episode ID | Primary TMDB Entry (Keep) | Duplicate TMDB Entry (Delete) | Title as Listed | Action for TMDB | Evidence & Provenance |
| :---: | :---: | :---: | :--- | :---: | :--- |
| [`MME00012`](episodes/MME00012.md) / [`MME00060`](episodes/MME00060.md) | [TMDB #1023000 (S02E07)](https://www.themoviedb.org/tv/6145-modern-marvels/season/2/episode/7) | [TMDB #1023046 (S05E19)](https://www.themoviedb.org/tv/6145-modern-marvels/season/5/episode/19) | **Statue of Liberty** | 🔴 **DELETE #1023046** | Re-entry of the 1995 premiere logged under a 1998 repeat date. Official streaming (History Vault #10571) anchors to 1995. |
| [`MME00026`](episodes/MME00026.md) / [`MME00057`](episodes/MME00057.md) | [TMDB #5138825 (S03E12)](https://www.themoviedb.org/tv/6145-modern-marvels/season/3/episode/12) | [TMDB #1023043 (S05E16)](https://www.themoviedb.org/tv/6145-modern-marvels/season/5/episode/16) | **The Alaskan Oil Pipeline** | 🔴 **DELETE #1023043** | Re-entry of the 1995 premiere logged under a 1998 rebroadcast date. Primary copyright card dates production to 1995. |
| [`MME00035`](episodes/MME00035.md) / [`MME00433`](episodes/MME00433.md) | [TMDB #1023015 (S04E05)](https://www.themoviedb.org/tv/6145-modern-marvels/season/4/episode/5) | [TMDB #1023793 (S11E76)](https://www.themoviedb.org/tv/6145-modern-marvels/season/11/episode/76) | **The Computer** | 🔴 **DELETE #1023793** | Re-entry of the 1996 premiere logged under a December 2004 repeat date. Streaming (History Vault #14272) anchors to 1996. |
| [`MME00090`](episodes/MME00090.md) / [`MME00263`](episodes/MME00263.md) | [TheTVDB #296792 (S06E12)](https://thetvdb.com/series/modern-marvels/episodes/296792) | [TMDB #1023241 (S09E57)](https://www.themoviedb.org/tv/6145-modern-marvels/season/9/episode/57) | **Salt Mines** | 🔴 **ALIGN TMDB AIR DATE** | Original broadcast occurred May 19, 1999. TMDB logged a December 2002 syndication repeat date as a new episode. |

---

### 3C. Cross-Database Desynchronizations (Air Date Splits Across TheTVDB & TMDB)

**What "Consolidate" means:**  
These are **not** duplicate entries within the same database. Instead, **TheTVDB** cataloged the episode under one air date/season (usually the original broadcast), while **TMDB** cataloged the *exact same documentary* under a completely different air date/season (usually a later syndication repeat).

Because the two databases had no link between these divergent dates, automated scrapers and our initial ingest pipeline created **two separate episode records** (`MME#####`) in the directory for the same physical documentary.

* **Action in this Archive:** We **consolidate** both records into a single master episode dossier (under the verified premiere date), cross-reference both database IDs in that master dossier, and deprecate the redundant duplicate MME ID.
* **Action for Upstream Databases:** TMDB should update its broadcast air date to match the verified original premiere, allowing media scrapers to recognize both listings describe the same film.

| Master Episode ID | Deprecated Duplicate ID | TheTVDB Listing (Verified Premiere) | TMDB Listing (Syndication Repeat) | Episode Title | Forensic Resolution & Action |
| :---: | :---: | :---: | :---: | :--- | :--- |
| [`MME00089`](episodes/MME00089.md) | `MME00258` | [TheTVDB #11742239](https://thetvdb.com/series/modern-marvels/episodes/11742239) (`1999-05-10`) | [TMDB #1023237 (S09E53)](https://www.themoviedb.org/tv/6145-modern-marvels/season/9/episode/53) (`2002-11-06`) | **Garbage** | Optical copyright cards date production to 1999 (`© MCMXCIX`). Archive consolidates under **MME00089**. TMDB must update its premiere date from 2002 to May 10, 1999. |
| [`MME00159`](episodes/MME00159.md) | `MME00333` | [TheTVDB #1335471 (S08E04)](https://thetvdb.com/series/modern-marvels/episodes/1335471) (`2001-01-20`) | [TMDB #1023313 (S10E64)](https://www.themoviedb.org/tv/6145-modern-marvels/season/10/episode/64) (`2003-10-25`) | **U-Boats** | Optical copyright cards date production to 2001 (`© 2001`). Archive consolidates under **MME00159**. TMDB must update its premiere date from 2003 to January 20, 2001. |
| [`MME00204`](episodes/MME00204.md) | `MME00268` / `MME00350` | [TheTVDB #11749825](https://thetvdb.com/series/modern-marvels/episodes/11749825) (`2002-01-02`) | [TMDB #1023244 (S09E60)](https://www.themoviedb.org/tv/6145-modern-marvels/season/9/episode/60) (`2002-12-05`) | **Failed Inventions** | Broadcast audio dates premiere to January 2, 2002. Archive consolidates under **MME00204**. TheTVDB duplicate #11749934 (2003) and TMDB repeat S09E60 (December 2002) must be linked to the January 2002 premiere. |

---

## 📅 Priority 4: Air Date Divergences & Forensic Transcript Analysis

Episodes where TheTVDB and TMDB diverge significantly, resolved via optical copyright cards and transcript temporal markers:

| Episode ID | Episode Title | TMDB Date | TheTVDB Date | Forensic Verdict | Primary Evidence Finding |
| :---: | :--- | :---: | :---: | :--- | :--- |
| [`MME00544`](episodes/MME00544.md) | **Shotguns** | [`2006-09-17` (TMDB #1023898)](https://www.themoviedb.org/tv/6145-modern-marvels/season/13/episode/38) | [`1999-05-23` (TVDB #320415)](https://thetvdb.com/series/modern-marvels/episodes/320415) | **Original 1999 production, re-packaged under Modern Marvels in 2006** | Primary optical credits prove this film was produced by Greystone Communications, Inc. under the on-screen title 'Tales of the Gun' with copyright '© MCMXCIX (1999) A&E Television Networks'. TheTVDB (1999-05-23) and IMDb (1999) record the genuine original premiere date. TMDB (2006-09-17, S13E38) records a syndication rebroadcast when The History Channel re-packaged several Greystone gun documentaries under the Modern Marvels umbrella. The copyright and production personnel confirm a 1999 origin, not 2006. |
| [`MME00107`](episodes/MME00107.md) | **More Earthmovers** | [`1999-10-18` (TMDB #1023086)](https://www.themoviedb.org/tv/6145-modern-marvels/season/6/episode/40) | [`2006-10-09` (TVDB #296643)](https://thetvdb.com/series/modern-marvels/episodes/296643) | **Revised 2006 cut incorporating post-2005 footage** | Optical copyright cards on the broadcast master carry dual years: '© 1999, 2005 Actuality Productions'. Crucially, transcript analysis reveals explicit dialogue referencing Hurricane Katrina: 'Hurricane Katrina made landfall in Mississippi on 29 August 2005...'. Because Katrina occurred in August 2005, the broadcast version cannot be the 1999 original. TheTVDB's air date of October 9, 2006 accurately dates this revised broadcast. |
| [`MME00243`](episodes/MME00243.md) | **Jet Engines** | [`2002-08-21` (TMDB #1023222)](https://www.themoviedb.org/tv/6145-modern-marvels/season/9/episode/38) | [`1999-05-03` (TVDB #296773)](https://thetvdb.com/series/modern-marvels/episodes/296773) | **Original 1999 production; TMDB reflects repeat** | Optical copyright card reads '© 1999 Actuality Productions'. Transcript internal dating confirms 1999 as the contemporary baseline: the narrator remarks 'no one would ever have anticipated that the airplane would have been flying in 1999, or as it probably will be in 2019' (treating 1999 as present and 2019 as future). TheTVDB's 1999-05-03 date is the verified original premiere. |
| [`MME00668`](episodes/MME00668.md) | **Helicopters** | [`2010-04-29` (TMDB #1024025)](https://www.themoviedb.org/tv/6145-modern-marvels/season/16/episode/12) | [`1998-09-14` (TVDB #296744)](https://thetvdb.com/series/modern-marvels/episodes/296744) | **Completely different 2010 HD documentary conflated with 1998 classic** | Optical copyright card reads '© 2009 Actuality Productions, Inc.'. Dialogue references 2008 production milestones: 'produce nearly 900 helicopters in 2008... winning Popular Science's Best of What's New award in 2008'. TheTVDB's 1998 date is an erroneous mapping to an earlier 1998 episode of the same name. TMDB's 2010-04-29 air date is correct. |
| [`MME00007`](episodes/MME00007.md) | **Balloons** | [`1994-12-16` (TMDB #1022994)](https://www.themoviedb.org/tv/6145-modern-marvels/season/2/episode/1) | [`1999-12-16` (TVDB #303329)](https://thetvdb.com/series/modern-marvels/episodes/303329) | **1999 production; TMDB date is erroneous** | Transcript dialogue discusses NASA exploration milestones scheduled for the future: 'NASA plans to launch its first interplanetary aerobot by rocket in 2003... scheduled to enter the atmosphere of Venus and Titan in 2005'. These plans were formulated in the late 1990s, refuting TMDB's 1994 date and confirming TheTVDB's December 1999 broadcast. |
| [`MME00573`](episodes/MME00573.md) | **More Ice** | [`2007-02-11` (TMDB #1023926)](https://www.themoviedb.org/tv/6145-modern-marvels/season/14/episode/6) | [`2009-10-28` (TVDB #693171)](https://thetvdb.com/series/modern-marvels/episodes/693171) | **2007 premiere; TheTVDB date is a late repeat** | Optical copyright card reads '© 2007 History Television Network Productions'. Transcript references research expeditions conducted in 2006: 'in 2006, scientists from California's Monterey Bay Aquarium Research Institute sailed to the Pacific coastal waters'. Corroborates TMDB's February 11, 2007 air date; TheTVDB's 2009 date is a syndicated repeat. |

---

## How to Submit Upstream Corrections

When submitting tickets to database moderators:
1. **TheTVDB:** Post a ticket at [support.thetvdb.com](https://support.thetvdb.com) referencing the specific Episode ID and citing the primary copyright year, dialogue transcript URL, and temporal evidence from this archive.
2. **TMDB:** Post a content report on the specific episode's discussion forum referencing the standalone 1-hour broadcast recordings.
3. **Link to Evidence:** Always provide the direct URL to the episode's dossier in this archive (`https://modernmarvelsfan.github.io/ModernMarvels/episodes/MME#####/`) as the primary proof.
