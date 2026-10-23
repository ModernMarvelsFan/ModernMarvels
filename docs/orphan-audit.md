# Modern Marvels: Single-Database Orphan Episodes Audit

> **Audit Date:** September 2, 2026  
> **Scope:** All 750 entries in the episode cross-reference directory.  
> **Summary:** Out of 750 episodes, 694 are corroborated by multiple independent databases. Exactly **56 entries** are either reported in only a single commercial database or carry no external database links. This audit categorizes each isolated entry to determine whether it represents an unverified single-database listing, a duplicate/rerun record, or a likely foreign/misattributed show.

---

## Summary of Findings

| Category | Count | Actionable Recommendation |
| :--- | :---: | :--- |
| **1. Likely Foreign / Misattributed Shows** | 2 | Flag as foreign/third-party imports incorrectly appended to the US Modern Marvels catalog; purge from directory. |
| **2. Duplicate & Rerun Records** | 18 | Merge with master episodes; deprecate phantom rerun IDs. |
| **3. Unique Episodes Indexed by Only One Database** | 36 | Retain in directory as single-database listings awaiting broadcast evidence. |

---

## 1. Likely Foreign / Misattributed Shows

Episodes originating from completely different television series that were mistakenly entered under *Modern Marvels* by upstream contributors:

### [`MME00171: How Did They Build That?: Concrete (2001-04-11)`](episodes/MME00171.md)
* **Reporting Database:** [TVDB #10579417](https://thetvdb.com/series/modern-marvels/episodes/10579417)
* **Evidence Corroboration:** Awaiting Evidence
* **Investigation Finding:** *'How Did They Build That?'* is an entirely separate architectural documentary series (specifically focusing on concrete structures) produced for the Smithsonian Channel and UK Channel 5 by Curve Media. History.com erroneously mislabeled an episode of this third-party series under the *Modern Marvels* banner. An upstream contributor viewed History.com as authoritative and cataloged it into TheTVDB under Modern Marvels Season 8.
* **Key Takeaway:** Official broadcaster web portals like History.com frequently contain metadata inaccuracies, repackaged syndication errors, and misattributed third-party acquisitions, and cannot be treated as a definitive or infallible source without independent corroboration.
* **Recommendation:** **Remove from Modern Marvels directory.**

### [`MME00731: World's Largest Cricket Stadium (2021-09-17)`](episodes/MME00731.md)
* **Reporting Database:** [TVDB #9277357](https://thetvdb.com/series/modern-marvels/episodes/9277357)
* **Evidence Corroboration:** Awaiting Evidence
* **Investigation Finding:** Produced and broadcast exclusively by regional affiliate *History TV18* in India as a standalone local special titled *'Modern Marvel: World's Largest Cricket Stadium'* (singular 'Marvel') focusing on the Narendra Modi Stadium in Ahmedabad. It was not produced by or affiliated with Actuality Productions / A+E Networks for the US series, and is not a true *Modern Marvels* episode. History TV18 mislabeled it under the series banner, and an upstream editor added it to TheTVDB.
* **Recommendation:** **Classify as an Indian regional spin-off/special; segregate from US series directory.**

---

## 2. Duplicate & Rerun Records

Entries that duplicate an existing episode under an altered title, secondary broadcast date, or rerun tag:

### [`MME00074: Firefighting! Containing the Demon (1998-12-07)`](episodes/MME00074.md)
* **Reporting Database:** [TVDB #10604100](https://thetvdb.com/series/modern-marvels/episodes/10604100)
* **Evidence Corroboration:** ✓
* **Duplicate Episode(s):** [`MME00506: Fire (2006-01-11)`](episodes/MME00506.md)

### [`MME00089: Garbage (1999-05-10)`](episodes/MME00089.md)
* **Reporting Database:** [TVDB #11742239](https://thetvdb.com/series/modern-marvels/episodes/11742239)
* **Evidence Corroboration:** Awaiting Evidence
* **Duplicate Episode(s):** [`MME00258: Garbage (2002-11-06)`](episodes/MME00258.md)
* **Investigation Finding:** *Garbage* was entered twice: once under TheTVDB (`1999-05-10`) and once under TMDB (`2002-11-06`). Both reference the identical documentary.
* **Recommendation:** **Consolidate into a single master entry.**

### [`MME00159: U-Boats (2001-01-20)`](episodes/MME00159.md)
* **Reporting Database:** [TVDB #1335471](https://thetvdb.com/series/modern-marvels/episodes/1335471)
* **Evidence Corroboration:** ✓
* **Duplicate Episode(s):** [`MME00333: U-Boats (2003-10-25)`](episodes/MME00333.md)
* **Investigation Finding:** *U-Boats* was entered twice under different season numbering across TheTVDB and TMDB.
* **Recommendation:** **Consolidate into a single master entry.**

### [`MME00207: Private Jets 2 (2002-01-28)`](episodes/MME00207.md)
* **Reporting Database:** [TVDB #296746](https://thetvdb.com/series/modern-marvels/episodes/296746)
* **Evidence Corroboration:** Awaiting Evidence
* **Duplicate Episode(s):** [`MME00211: Private Jets (2002-02-01)`](episodes/MME00211.md)

### [`MME00258: Garbage (2002-11-06)`](episodes/MME00258.md)
* **Reporting Database:** [TMDB #1023237 (S09E53)](https://www.themoviedb.org/tv/6145-modern-marvels/season/9/episode/53)
* **Evidence Corroboration:** Awaiting Evidence
* **Duplicate Episode(s):** [`MME00089: Garbage (1999-05-10)`](episodes/MME00089.md)
* **Investigation Finding:** *Garbage* was entered twice: once under TheTVDB (`1999-05-10`) and once under TMDB (`2002-11-06`). Both reference the identical documentary.
* **Recommendation:** **Consolidate into a single master entry.**

### [`MME00266: Boys' Toys - Motorcycles (2002-12-03)`](episodes/MME00266.md)
* **Reporting Database:** [TVDB #7696202](https://thetvdb.com/series/modern-marvels/episodes/7696202)
* **Evidence Corroboration:** Awaiting Evidence
* **Duplicate Episode(s):** [`MME00110: Motorcycles (1999-11-15)`](episodes/MME00110.md), [`MME00265: Motorcycles (2002-12-03)`](episodes/MME00265.md), [`MME00354: Toys (2003-12-23)`](episodes/MME00354.md)

### [`MME00282: Japanese Guns of WWII (2003-03-26)`](episodes/MME00282.md)
* **Reporting Database:** [TMDB #1023263 (S10E14)](https://www.themoviedb.org/tv/6145-modern-marvels/season/10/episode/14)
* **Evidence Corroboration:** Awaiting Evidence
* **Duplicate Episode(s):** [`MME00397: Guns of WWII (2004-09-17)`](episodes/MME00397.md)

### [`MME00327: Early Machine Guns (2003-09-26)`](episodes/MME00327.md)
* **Reporting Database:** [TMDB #1023307 (S10E58)](https://www.themoviedb.org/tv/6145-modern-marvels/season/10/episode/58)
* **Evidence Corroboration:** Awaiting Evidence
* **Duplicate Episode(s):** [`MME00287: Machine Guns (2003-04-30)`](episodes/MME00287.md)

### [`MME00333: U-Boats (2003-10-25)`](episodes/MME00333.md)
* **Reporting Database:** [TMDB #1023313 (S10E64)](https://www.themoviedb.org/tv/6145-modern-marvels/season/10/episode/64)
* **Evidence Corroboration:** Awaiting Evidence
* **Duplicate Episode(s):** [`MME00159: U-Boats (2001-01-20)`](episodes/MME00159.md)
* **Investigation Finding:** *U-Boats* was entered twice under different season numbering across TheTVDB and TMDB.
* **Recommendation:** **Consolidate into a single master entry.**

### [`MME00350: Failed Inventions (2003-12-10)`](episodes/MME00350.md)
* **Reporting Database:** [TVDB #11749934](https://thetvdb.com/series/modern-marvels/episodes/11749934)
* **Evidence Corroboration:** Awaiting Evidence
* **Duplicate Episode(s):** [`MME00204: Failed Inventions (2002-01-02)`](episodes/MME00204.md), [`MME00268: Failed Inventions (2002-12-05)`](episodes/MME00268.md)
* **Investigation Finding:** *Failed Inventions* was entered twice under TheTVDB and TMDB with different re-run dates.
* **Recommendation:** **Consolidate into a single master entry.**

### [`MME00438: Nature's Engineers 2 (2005-01-18)`](episodes/MME00438.md)
* **Reporting Database:** [TVDB #11750035](https://thetvdb.com/series/modern-marvels/episodes/11750035)
* **Evidence Corroboration:** Awaiting Evidence
* **Duplicate Episode(s):** [`MME00366: Nature's Engineers (2004-03-31)`](episodes/MME00366.md), [`MME00375: Nature's Engineers (2004-05-31)`](episodes/MME00375.md)

### [`MME00440: Blackbird Stealth (2005-02-04)`](episodes/MME00440.md)
* **Reporting Database:** [TMDB #1023800 (S12E06)](https://www.themoviedb.org/tv/6145-modern-marvels/season/12/episode/6)
* **Evidence Corroboration:** Awaiting Evidence
* **Duplicate Episode(s):** [`MME00565: Tea (2006-12-13)`](episodes/MME00565.md)

### [`MME00458: The Golden Gate Bridge (2) (2005-05-11)`](episodes/MME00458.md)
* **Reporting Database:** [TVDB #7930503](https://thetvdb.com/series/modern-marvels/episodes/7930503)
* **Evidence Corroboration:** Awaiting Evidence
* **Duplicate Episode(s):** [`MME00017: The Golden Gate Bridge (1995-05-21)`](episodes/MME00017.md)
* **Investigation Finding:** Upstream TheTVDB contributor created duplicate entries appending '(2)' for later rebroadcasts.
* **Recommendation:** **Merge into primary master episode.**

### [`MME00519: The Telephone (2) (2006-05-07)`](episodes/MME00519.md)
* **Reporting Database:** [TVDB #7930575](https://thetvdb.com/series/modern-marvels/episodes/7930575)
* **Evidence Corroboration:** Awaiting Evidence
* **Duplicate Episode(s):** [`MME00032: The Telephone (1996-09-15)`](episodes/MME00032.md)
* **Investigation Finding:** Upstream TheTVDB contributor created duplicate entries appending '(2)' for later rebroadcasts.
* **Recommendation:** **Merge into primary master episode.**

### [`MME00552: Stealth & Beyond: Air Stealth (2006-09-27)`](episodes/MME00552.md)
* **Reporting Database:** [TMDB #1023905 (S13E45)](https://www.themoviedb.org/tv/6145-modern-marvels/season/13/episode/45)
* **Evidence Corroboration:** Awaiting Evidence
* **Duplicate Episode(s):** [`MME00565: Tea (2006-12-13)`](episodes/MME00565.md)

### [`MME00750: The Sears Tower (2024-10-13)`](episodes/MME00750.md)
* **Reporting Database:** [TVDB #11755189](https://thetvdb.com/series/modern-marvels/episodes/11755189)
* **Evidence Corroboration:** Awaiting Evidence
* **Duplicate Episode(s):** [`MME00395: The Sears Tower (2004-09-08)`](episodes/MME00395.md)
* **Investigation Finding:** Erroneously added to TheTVDB with a 2024 air date (`2024-10-13`). Modern Marvels original production concluded in 2022. This is a duplicate rerun entry of the original 2004 documentary *The Sears Tower* (`MME00395`).
* **Recommendation:** **Merge into `MME00395`; remove `MME00750`.**

### [`MME00751: More Helicopters ()`](episodes/MME00751.md)
* **Reporting Database:** [TVDB #320421](https://thetvdb.com/series/modern-marvels/episodes/320421)
* **Evidence Corroboration:** Awaiting Evidence
* **Duplicate Episode(s):** [`MME00210: Helicopters (2002-01-31)`](episodes/MME00210.md), [`MME00668: Helicopters (2010-04-29)`](episodes/MME00668.md)

### [`MME00754: Greatest Movie Gadgets (2004-06-17)`](episodes/MME00754.md)
* **Reporting Database:** [IMDb #tt1055721](https://www.imdb.com/title/tt1055721/)
* **Evidence Corroboration:** ✓
* **Duplicate Episode(s):** [`MME00123: Gadgets (2000-03-13)`](episodes/MME00123.md)

---

## 3. Unique Episodes Indexed by Only One Database

These entries are indexed by only a single commercial database (often because TheTVDB or TMDB had a blind spot for certain military or technology specials). They lack multi-database corroboration and have not been independently confirmed across multiple catalogues:

| Episode ID | Title | Claimed Air Date | Sole Database | Evidence Corroboration |
| :--- | :--- | :---: | :---: | :---: |
| [`MME00029`](episodes/MME00029.md) | **America's Highways** | 1996-09-02 | [TMDB #1023011 (S04E01)](https://www.themoviedb.org/tv/6145-modern-marvels/season/4/episode/1) | Awaiting Evidence |
| [`MME00037`](episodes/MME00037.md) | **Camera** | 1996-12-15 | [TheTVDB #4504642 (S00E107)](https://thetvdb.com/series/modern-marvels/episodes/4504642) | Awaiting Evidence |
| [`MME00064`](episodes/MME00064.md) | **World's Fair: Visions of the Future** | 1998-09-24 | [TheTVDB #10606850 (S05E05)](https://thetvdb.com/series/modern-marvels/episodes/10606850) | Awaiting Evidence |
| [`MME00068`](episodes/MME00068.md) | **Monumental Statues** | 1998-10-28 | [TMDB #1023053 (S06E07)](https://www.themoviedb.org/tv/6145-modern-marvels/season/6/episode/7) | Awaiting Evidence |
| [`MME00116`](episodes/MME00116.md) | **Wartime Aircraft Production WWII** | 2000-01-01 | [TheTVDB #6523649 (S00E31)](https://thetvdb.com/series/modern-marvels/episodes/6523649) | Awaiting Evidence |
| [`MME00143`](episodes/MME00143.md) | **The Quest for Muscle** | 2000-09-26 | [TheTVDB #7855437 (S07E27)](https://thetvdb.com/series/modern-marvels/episodes/7855437) | Awaiting Evidence |
| [`MME00176`](episodes/MME00176.md) | **Extreme Planes** | 2001-05-22 | [TheTVDB #4262613 (S00E06)](https://thetvdb.com/series/modern-marvels/episodes/4262613) | Awaiting Evidence |
| [`MME00191`](episodes/MME00191.md) | **The Mig** | 2001-09-27 | [TheTVDB #977151](https://thetvdb.com/series/modern-marvels/episodes/977151) | Awaiting Evidence |
| [`MME00225`](episodes/MME00225.md) | **Big Rigs of Combat: Jeeps** | 2002-06-02 | [TheTVDB #9262279 (S09E19)](https://thetvdb.com/series/modern-marvels/episodes/9262279) | ✓ |
| [`MME00246`](episodes/MME00246.md) | **Liberty Ships of World War II** | 2002-09-10 | [TMDB #1023225 (S09E41)](https://www.themoviedb.org/tv/6145-modern-marvels/season/9/episode/41) | Awaiting Evidence |
| [`MME00339`](episodes/MME00339.md) | **Guns of the Sky** | 2003-11-07 | [TMDB #1023319 (S10E70)](https://www.themoviedb.org/tv/6145-modern-marvels/season/10/episode/70) | Awaiting Evidence |
| [`MME00343`](episodes/MME00343.md) | **Million Dollar Cars** | 2003-11-26 | [TMDB #1023323 (S10E74)](https://www.themoviedb.org/tv/6145-modern-marvels/season/10/episode/74) | Awaiting Evidence |
| [`MME00344`](episodes/MME00344.md) | **B-52: Stratofortress** | 2003-11-28 | [TMDB #1023325 (S10E76)](https://www.themoviedb.org/tv/6145-modern-marvels/season/10/episode/76) | Awaiting Evidence |
| [`MME00346`](episodes/MME00346.md) | **Rolls Royce** | 2003-12-02 | [TMDB #1023327 (S10E78)](https://www.themoviedb.org/tv/6145-modern-marvels/season/10/episode/78) | Awaiting Evidence |
| [`MME00348`](episodes/MME00348.md) | **Wheel Estate** | 2003-12-03 | [TMDB #1023329 (S10E80)](https://www.themoviedb.org/tv/6145-modern-marvels/season/10/episode/80) | Awaiting Evidence |
| [`MME00361`](episodes/MME00361.md) | **Ship of Gold** | 2004-02-13 | [TMDB #1023723 (S11E06)](https://www.themoviedb.org/tv/6145-modern-marvels/season/11/episode/6) | Awaiting Evidence |
| [`MME00373`](episodes/MME00373.md) | **The Subs of WWII** | 2004-05-20 | [TMDB #1023735 (S11E18)](https://www.themoviedb.org/tv/6145-modern-marvels/season/11/episode/18) | Awaiting Evidence |
| [`MME00397`](episodes/MME00397.md) | **Guns of WWII** | 2004-09-17 | [TMDB #1023760 (S11E41)](https://www.themoviedb.org/tv/6145-modern-marvels/season/11/episode/41) | Awaiting Evidence |
| [`MME00421`](episodes/MME00421.md) | **Movie Theaters** | 2004-11-24 | [TMDB #1023781 (S11E64)](https://www.themoviedb.org/tv/6145-modern-marvels/season/11/episode/64) | Awaiting Evidence |
| [`MME00426`](episodes/MME00426.md) | **Heavy Metal: PT Boat** | 2004-12-17 | [TheTVDB #11750053 (S11E64)](https://thetvdb.com/series/modern-marvels/episodes/11750053) | Awaiting Evidence |
| [`MME00465`](episodes/MME00465.md) | **Secret Japanese Aircraft of World War II** | 2005-06-16 | [TMDB #1023823 (S12E30)](https://www.themoviedb.org/tv/6145-modern-marvels/season/12/episode/30) | Awaiting Evidence |
| [`MME00469`](episodes/MME00469.md) | **Independence Day: The History Of The 4th Of July** | 2005-07-04 | [TheTVDB #4262611 (S00E17)](https://thetvdb.com/series/modern-marvels/episodes/4262611) | Awaiting Evidence |
| [`MME00478`](episodes/MME00478.md) | **Secret Luftwaffe Aircraft of World War II** | 2005-08-17 | [TMDB #1023835 (S12E42)](https://www.themoviedb.org/tv/6145-modern-marvels/season/12/episode/42) | ✓ |
| [`MME00481`](episodes/MME00481.md) | **High Risk: Helicopter Lineman** | 2005-08-31 | [TMDB #1023839 (S12E45)](https://www.themoviedb.org/tv/6145-modern-marvels/season/12/episode/45) | Awaiting Evidence |
| [`MME00485`](episodes/MME00485.md) | **Engineering an Empire: Rome** | 2005-09-13 | [TMDB #1023843 (S12E49)](https://www.themoviedb.org/tv/6145-modern-marvels/season/12/episode/49) | Awaiting Evidence |
| [`MME00490`](episodes/MME00490.md) | **German Small Arms of World War II** | 2005-09-24 | [TMDB #1023848 (S12E54)](https://www.themoviedb.org/tv/6145-modern-marvels/season/12/episode/54) | ✓ |
| [`MME00497`](episodes/MME00497.md) | **Secret Russian Aircraft of WWII** | 2005-11-30 | [TheTVDB #4111305 (S00E106)](https://thetvdb.com/series/modern-marvels/episodes/4111305) | Awaiting Evidence |
| [`MME00518`](episodes/MME00518.md) | **Google: Behind the Screen** | 2006-05-07 | [TheTVDB #4262610 (S00E18)](https://thetvdb.com/series/modern-marvels/episodes/4262610) | Awaiting Evidence |
| [`MME00527`](episodes/MME00527.md) | **American Eats Special** | 2006-07-02 | [TMDB #1023881 (S13E21)](https://www.themoviedb.org/tv/6145-modern-marvels/season/13/episode/21) | Awaiting Evidence |
| [`MME00535`](episodes/MME00535.md) | **Classic Cars** | 2006-08-03 | [TMDB #1023889 (S13E29)](https://www.themoviedb.org/tv/6145-modern-marvels/season/13/episode/29) | Awaiting Evidence |
| [`MME00536`](episodes/MME00536.md) | **Making Medieval Armor** | 2006-08-03 | [TMDB #1023890 (S13E30)](https://www.themoviedb.org/tv/6145-modern-marvels/season/13/episode/30) | Awaiting Evidence |
| [`MME00537`](episodes/MME00537.md) | **Rube Goldberg** | 2006-08-03 | [TMDB #1023891 (S13E31)](https://www.themoviedb.org/tv/6145-modern-marvels/season/13/episode/31) | Awaiting Evidence |
| [`MME00598`](episodes/MME00598.md) | **Nature Tech: Volcanoes** | 2007-08-29 | [TMDB #1023951 (S14E31)](https://www.themoviedb.org/tv/6145-modern-marvels/season/14/episode/31) | Awaiting Evidence |
| [`MME00659`](episodes/MME00659.md) | **De Havilland Mosquito** | 2010-01-29 | [TheTVDB #4262621 (S00E20)](https://thetvdb.com/series/modern-marvels/episodes/4262621) | ✓ |
| [`MME00676`](episodes/MME00676.md) | **Most Extreme Airports** | 2010-07-20 | [TheTVDB #11903056 (S00E116)](https://thetvdb.com/series/modern-marvels/episodes/11903056) | Awaiting Evidence |
| [`MME00753`](episodes/MME00753.md) | **B-17 Flying Fortress** |  | [TheTVDB #7312645 (S00E102)](https://thetvdb.com/series/modern-marvels/episodes/7312645) | Awaiting Evidence |
