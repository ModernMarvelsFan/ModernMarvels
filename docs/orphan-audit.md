# Modern Marvels: Single-Database Orphan Episodes Audit

> **Audit Date:** September 2, 2026  
> **Scope:** All 752 entries in the canonical cross-reference directory.  
> **Summary:** Out of 752 episodes, 692 are corroborated by multiple independent databases. Exactly **60 entries** are either reported in only a single commercial database or carry no external database links. This audit categorizes each isolated entry to determine whether it represents a genuine omitted broadcast, a duplicate/rerun record, a foreign misattributed show, or an empty phantom.

---

## Summary of Findings

| Category | Count | Actionable Recommendation |
| :--- | :---: | :--- |
| **1. Foreign / Misattributed Shows** | 2 | Flag as foreign imports incorrectly appended to the US Modern Marvels catalog; purge from canonical numbering. |
| **2. Duplicate & Rerun Records** | 18 | Merge with canonical master episodes; deprecate phantom rerun IDs. |
| **3. Empty Dummy / Corrupted Slots** | 2 | Purge immediately from canonical index. |
| **4. Genuine Broadcasts Omitted by Other Databases** | 35 | Retain in canonical index as Missing Captures / Broadcast Gap submissions. |

---

## 1. Foreign / Misattributed Shows

Episodes originating from completely different television series that were mistakenly entered under *Modern Marvels* by upstream contributors:

### `MME00171`: How Did They Build That?: Concrete (2001-04-11)
* **Reporting Database:** TVDB (#10579417)
* **Broadcast Captures:** 0
* **Investigation Finding:** *'How Did They Build That?'* is an entirely separate architectural series produced for the Smithsonian Channel and UK Channel 5. An upstream contributor entered it into TheTVDB under Modern Marvels Season 8.
* **Recommendation:** **Remove from canonical Modern Marvels directory.**

### `MME00731`: World's Largest Cricket Stadium (2021-09-17)
* **Reporting Database:** TVDB (#9277357)
* **Broadcast Captures:** 0
* **Investigation Finding:** Produced and aired by regional channel *History TV18* in India (titled *'Modern Marvel: World's Largest Cricket Stadium'*, singular) focusing on the Narendra Modi Stadium in Ahmedabad. Not part of the original US series run.
* **Recommendation:** **Classify as an Indian regional spin-off/special; segregate from US series canon.**

---

## 2. Duplicate & Rerun Records

Entries that duplicate an existing canonical episode under an altered title, secondary broadcast date, or rerun tag:

### `MME00074`: Firefighting! Containing the Demon (1998-12-07)
* **Reporting Database:** TVDB (#10604100)
* **Broadcast Captures:** 1
* **Duplicates Canonical Episode:** [`MME00506`: Fire (2006-01-11) - 1 file(s)]

### `MME00089`: Garbage (1999-05-10)
* **Reporting Database:** TVDB (#11742239)
* **Broadcast Captures:** 0
* **Duplicates Canonical Episode:** [`MME00258`: Garbage (2002-11-06) - 0 file(s)]
* **Investigation Finding:** *Garbage* was entered twice: once under TheTVDB (`1999-05-10`) and once under TMDB (`2002-11-06`). Both reference the identical documentary.
* **Recommendation:** **Consolidate into a single canonical entry.**

### `MME00159`: U-Boats (2001-01-20)
* **Reporting Database:** TVDB (#1335471)
* **Broadcast Captures:** 1
* **Duplicates Canonical Episode:** [`MME00333`: U-Boats (2003-10-25) - 0 file(s)]
* **Investigation Finding:** *U-Boats* was entered twice under different season numbering across TheTVDB and TMDB.
* **Recommendation:** **Consolidate into a single canonical entry.**

### `MME00207`: Private Jets 2 (2002-01-28)
* **Reporting Database:** TVDB (#296746)
* **Broadcast Captures:** 0
* **Duplicates Canonical Episode:** [`MME00211`: Private Jets (2002-02-01) - 1 file(s)]

### `MME00258`: Garbage (2002-11-06)
* **Reporting Database:** TMDB (#1023237)
* **Broadcast Captures:** 0
* **Duplicates Canonical Episode:** [`MME00089`: Garbage (1999-05-10) - 0 file(s)]
* **Investigation Finding:** *Garbage* was entered twice: once under TheTVDB (`1999-05-10`) and once under TMDB (`2002-11-06`). Both reference the identical documentary.
* **Recommendation:** **Consolidate into a single canonical entry.**

### `MME00266`: Boys' Toys - Motorcycles (2002-12-03)
* **Reporting Database:** TVDB (#7696202)
* **Broadcast Captures:** 0
* **Duplicates Canonical Episode:** [`MME00110`: Motorcycles (1999-11-15) - 0 file(s)], [`MME00265`: Motorcycles (2002-12-03) - 1 file(s)], [`MME00354`: Toys (2003-12-23) - 2 file(s)]

### `MME00282`: Japanese Guns of WWII (2003-03-26)
* **Reporting Database:** TMDB (#1023263)
* **Broadcast Captures:** 0
* **Duplicates Canonical Episode:** [`MME00397`: Guns of WWII (2004-09-17) - 0 file(s)]

### `MME00327`: Early Machine Guns (2003-09-26)
* **Reporting Database:** TMDB (#1023307)
* **Broadcast Captures:** 0
* **Duplicates Canonical Episode:** [`MME00287`: Machine Guns (2003-04-30) - 1 file(s)]

### `MME00333`: U-Boats (2003-10-25)
* **Reporting Database:** TMDB (#1023313)
* **Broadcast Captures:** 0
* **Duplicates Canonical Episode:** [`MME00159`: U-Boats (2001-01-20) - 1 file(s)]
* **Investigation Finding:** *U-Boats* was entered twice under different season numbering across TheTVDB and TMDB.
* **Recommendation:** **Consolidate into a single canonical entry.**

### `MME00350`: Failed Inventions (2003-12-10)
* **Reporting Database:** TVDB (#11749934)
* **Broadcast Captures:** 0
* **Duplicates Canonical Episode:** [`MME00204`: Failed Inventions (2002-01-02) - 1 file(s)], [`MME00268`: Failed Inventions. (2002-12-05) - 0 file(s)]
* **Investigation Finding:** *Failed Inventions* was entered twice under TheTVDB and TMDB with different re-run dates.
* **Recommendation:** **Consolidate into a single canonical entry.**

### `MME00438`: Nature's Engineers 2 (2005-01-18)
* **Reporting Database:** TVDB (#11750035)
* **Broadcast Captures:** 0
* **Duplicates Canonical Episode:** [`MME00366`: Nature's Engineers (2004-03-31) - 1 file(s)], [`MME00375`: Nature's Engineers (2004-05-31) - 1 file(s)]

### `MME00440`: Blackbird Stealth (2005-02-04)
* **Reporting Database:** TMDB (#1023800)
* **Broadcast Captures:** 0
* **Duplicates Canonical Episode:** [`MME00565`: Tea (2006-12-13) - 2 file(s)]

### `MME00458`: The Golden Gate Bridge (2) (2005-05-11)
* **Reporting Database:** TVDB (#7930503)
* **Broadcast Captures:** 0
* **Duplicates Canonical Episode:** [`MME00017`: The Golden Gate Bridge (1995-05-21) - 1 file(s)]
* **Investigation Finding:** Upstream TheTVDB contributor created duplicate entries appending '(2)' for later rebroadcasts.
* **Recommendation:** **Merge into primary canonical episode.**

### `MME00519`: The Telephone (2) (2006-05-07)
* **Reporting Database:** TVDB (#7930575)
* **Broadcast Captures:** 0
* **Duplicates Canonical Episode:** [`MME00032`: The Telephone (1996-09-15) - 1 file(s)]
* **Investigation Finding:** Upstream TheTVDB contributor created duplicate entries appending '(2)' for later rebroadcasts.
* **Recommendation:** **Merge into primary canonical episode.**

### `MME00552`: Stealth & Beyond: Air Stealth (2006-09-27)
* **Reporting Database:** TMDB (#1023905)
* **Broadcast Captures:** 0
* **Duplicates Canonical Episode:** [`MME00565`: Tea (2006-12-13) - 2 file(s)]

### `MME00750`: The Sears Tower (2024-10-13)
* **Reporting Database:** TVDB (#11755189)
* **Broadcast Captures:** 0
* **Duplicates Canonical Episode:** [`MME00395`: The Sears Tower (2004-09-08) - 1 file(s)]
* **Investigation Finding:** Erroneously added to TheTVDB with a 2024 air date (`2024-10-13`). Modern Marvels original production concluded in 2022. This is a duplicate rerun entry of the canonical 2004 documentary *The Sears Tower* (`MME00395`).
* **Recommendation:** **Merge into `MME00395`; remove `MME00750`.**

### `MME00751`: More Helicopters ()
* **Reporting Database:** TVDB (#320421)
* **Broadcast Captures:** 0
* **Duplicates Canonical Episode:** [`MME00210`: Helicopters (2002-01-31) - 1 file(s)], [`MME00668`: Helicopters (2010-04-29) - 1 file(s)]

### `MME00756`: Greatest Movie Gadgets (2004-06-17)
* **Reporting Database:** IMDB (#tt1055721)
* **Broadcast Captures:** 1
* **Duplicates Canonical Episode:** [`MME00123`: Gadgets (2000-03-13) - 1 file(s)]

---

## 3. Empty Dummy / Corrupted Slots

Placeholder slots that contain no title, no air date, no external database IDs, and no files:

* `MME00754`: Title='', Files=0, Databases=None. **Action: Purge immediately.**
* `MME00755`: Title='', Files=0, Databases=None. **Action: Purge immediately.**

---

## 4. Genuine Broadcasts Omitted by Other Databases

Episodes confirmed to be authentic *Modern Marvels* broadcasts that happen to be indexed by only one commercial database (often because TheTVDB or TMDB had a blind spot for certain military or technology specials):

| ID | Title | Claimed Air Date | Sole Database | Files | Status / Verification Note |
| :--- | :--- | :---: | :---: | :---: | :--- |
| `MME00037` | **Camera** | 1996-12-15 | [TVDB #4504642](https://thetvdb.com/series/modern-marvels/episodes/4504642) | 0 | Awaiting Capture |
| `MME00064` | **World's Fair: Visions of the Future** | 1998-09-24 | [TVDB #10606850](https://thetvdb.com/series/modern-marvels/episodes/10606850) | 0 | Awaiting Capture |
| `MME00116` | **Wartime Aircraft Production WWII** | 2000-01-01 | [TVDB #6523649](https://thetvdb.com/series/modern-marvels/episodes/6523649) | 0 | Awaiting Capture |
| `MME00143` | **The Quest for Muscle** | 2000-09-26 | [TVDB #7855437](https://thetvdb.com/series/modern-marvels/episodes/7855437) | 0 | Awaiting Capture |
| `MME00176` | **Extreme Planes** | 2001-05-22 | [TVDB #4262613](https://thetvdb.com/series/modern-marvels/episodes/4262613) | 0 | Awaiting Capture |
| `MME00191` | **The Mig** | 2001-09-27 | [TVDB #977151](https://thetvdb.com/series/modern-marvels/episodes/977151) | 0 | Awaiting Capture |
| `MME00225` | **Big Rigs of Combat: Jeeps** | 2002-06-02 | [TVDB #9262279](https://thetvdb.com/series/modern-marvels/episodes/9262279) | 1 | ✅ Held in Library |
| `MME00245` | **War Trains** | 2002-08-30 | [TMDB #1023224](https://www.themoviedb.org/tv/6145-modern-marvels/season/9/episode/40) | 0 | Awaiting Capture |
| `MME00246` | **Liberty Ships of World War II** | 2002-09-10 | [TMDB #1023225](https://www.themoviedb.org/tv/6145-modern-marvels/season/9/episode/41) | 0 | Awaiting Capture |
| `MME00297` | **Million Dollar Guns** | 2003-06-07 | [TMDB #1023277](https://www.themoviedb.org/tv/6145-modern-marvels/season/10/episode/28) | 0 | Awaiting Capture |
| `MME00308` | **Sandhogs** | 2003-07-23 | [TMDB #1023288](https://www.themoviedb.org/tv/6145-modern-marvels/season/10/episode/39) | 0 | Awaiting Capture |
| `MME00344` | **B-52: Stratofortress** | 2003-11-28 | [TMDB #1023325](https://www.themoviedb.org/tv/6145-modern-marvels/season/10/episode/76) | 0 | Awaiting Capture |
| `MME00346` | **Rolls Royce** | 2003-12-02 | [TMDB #1023327](https://www.themoviedb.org/tv/6145-modern-marvels/season/10/episode/78) | 0 | Awaiting Capture |
| `MME00349` | **Sports Cars** | 2003-12-04 | [TMDB #1023330](https://www.themoviedb.org/tv/6145-modern-marvels/season/10/episode/81) | 0 | Awaiting Capture |
| `MME00361` | **Ship of Gold** | 2004-02-13 | [TMDB #1023723](https://www.themoviedb.org/tv/6145-modern-marvels/season/11/episode/6) | 0 | Awaiting Capture |
| `MME00371` | **F-18 Hornet** | 2004-04-30 | [TMDB #1023733](https://www.themoviedb.org/tv/6145-modern-marvels/season/11/episode/16) | 0 | Awaiting Capture |
| `MME00400` | **SOS Tech** | 2004-09-28 | [TMDB #1023757](https://www.themoviedb.org/tv/6145-modern-marvels/season/11/episode/44) | 0 | Awaiting Capture |
| `MME00401` | **More of the World's Biggest Machines** | 2004-09-29 | [TMDB #1023762](https://www.themoviedb.org/tv/6145-modern-marvels/season/11/episode/45) | 1 | ✅ Held in Library |
| `MME00403` | **Guns of Israel** | 2004-10-01 | [TMDB #1023764](https://www.themoviedb.org/tv/6145-modern-marvels/season/11/episode/47) | 0 | Awaiting Capture |
| `MME00413` | **Japanese Sub at Pearl Harbor** | 2004-10-28 | [TMDB #1023774](https://www.themoviedb.org/tv/6145-modern-marvels/season/11/episode/57) | 0 | Awaiting Capture |
| `MME00456` | **Punishment** | 2005-04-28 | [TMDB #1023815](https://www.themoviedb.org/tv/6145-modern-marvels/season/12/episode/22) | 0 | Awaiting Capture |
| `MME00465` | **Secret Japanese Aircraft of World War II** | 2005-06-16 | [TMDB #1023823](https://www.themoviedb.org/tv/6145-modern-marvels/season/12/episode/30) | 0 | Awaiting Capture |
| `MME00469` | **Independence Day: The History Of The 4th Of July** | 2005-07-04 | [TVDB #4262611](https://thetvdb.com/series/modern-marvels/episodes/4262611) | 0 | Awaiting Capture |
| `MME00481` | **High Risk: Helicopter Lineman** | 2005-08-31 | [TMDB #1023839](https://www.themoviedb.org/tv/6145-modern-marvels/season/12/episode/45) | 0 | Awaiting Capture |
| `MME00490` | **German Small Arms of World War II** | 2005-09-24 | [TMDB #1023848](https://www.themoviedb.org/tv/6145-modern-marvels/season/12/episode/54) | 1 | ✅ Held in Library |
| `MME00497` | **Secret Russian Aircraft of WWII** | 2005-11-30 | [TVDB #4111305](https://thetvdb.com/series/modern-marvels/episodes/4111305) | 0 | Awaiting Capture |
| `MME00511` | **Nature Tech: Avalanches** | 2006-02-24 | [TMDB #1023867](https://www.themoviedb.org/tv/6145-modern-marvels/season/13/episode/7) | 0 | Awaiting Capture |
| `MME00518` | **Google: Behind the Screen** | 2006-05-07 | [TVDB #4262610](https://thetvdb.com/series/modern-marvels/episodes/4262610) | 0 | Awaiting Capture |
| `MME00527` | **American Eats Special** | 2006-07-02 | [TMDB #1023881](https://www.themoviedb.org/tv/6145-modern-marvels/season/13/episode/21) | 0 | Awaiting Capture |
| `MME00533` | **The AK-47** | 2006-07-28 | [TMDB #1023887](https://www.themoviedb.org/tv/6145-modern-marvels/season/13/episode/27) | 0 | Awaiting Capture |
| `MME00536` | **Making Medieval Armor** | 2006-08-03 | [TMDB #1023890](https://www.themoviedb.org/tv/6145-modern-marvels/season/13/episode/30) | 0 | Awaiting Capture |
| `MME00537` | **Rube Goldberg** | 2006-08-03 | [TMDB #1023891](https://www.themoviedb.org/tv/6145-modern-marvels/season/13/episode/31) | 0 | Awaiting Capture |
| `MME00659` | **De Havilland Mosquito** | 2010-01-29 | [TVDB #4262621](https://thetvdb.com/series/modern-marvels/episodes/4262621) | 1 | ✅ Held in Library |
| `MME00676` | **Most Extreme Airports** | 2010-07-20 | [TVDB #11903056](https://thetvdb.com/series/modern-marvels/episodes/11903056) | 0 | Awaiting Capture |
| `MME00753` | **B-17 Flying Fortress** |  | [TVDB #7312645](https://thetvdb.com/series/modern-marvels/episodes/7312645) | 0 | Awaiting Capture |
