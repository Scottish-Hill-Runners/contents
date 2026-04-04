# Race CSV Discrepancies

Scanned **2063** files; **109** files have issues. **57** header issues, **185** unique row issues (415 total occurrences).

## `races/Birnam/2021.csv`

**Header issues:**

- Non-standard column name `FinishPosition` (expected `RunnerPosition`)

## `races/Birnam/2022.csv`

**Header issues:**

- Non-standard column name `FinishPosition` (expected `RunnerPosition`)

## `races/Birnam/2023.csv`

**Header issues:**

- Non-standard column name `FinishPosition` (expected `RunnerPosition`)

## `races/CaerkettonHillRace/2014***.csv`

**Row issues (28 unique, 102 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | FinishTime | `Belahouston` | Not in (h:)mm:ss format | 10 |
| 1 | FinishTime | `Calderglen Harriers` | Not in (h:)mm:ss format | 56 |
| 2 | FinishTime | `Carnegie` | Not in (h:)mm:ss format | 75, 99 |
| 27 | FinishTime | `Carnethy` | Not in (h:)mm:ss format | 3, 4, 5, 9, 13, 15, 17, 19, 20, 21, … (+17) |
| 5 | FinishTime | `Corstorphine` | Not in (h:)mm:ss format | 7, 12, 43, 55, 89 |
| 1 | FinishTime | `Drumore` | Not in (h:)mm:ss format | 34 |
| 1 | FinishTime | `Dunbar` | Not in (h:)mm:ss format | 26 |
| 2 | FinishTime | `Edinburgh AC` | Not in (h:)mm:ss format | 51, 72 |
| 1 | FinishTime | `Fat Boys` | Not in (h:)mm:ss format | 53 |
| 1 | FinishTime | `Glasgow Hares & Hounds` | Not in (h:)mm:ss format | 28 |
| 10 | FinishTime | `HBT` | Not in (h:)mm:ss format | 2, 8, 18, 23, 31, 33, 35, 39, 61, 84 |
| 2 | FinishTime | `Helensburgh` | Not in (h:)mm:ss format | 36, 62 |
| 1 | FinishTime | `Helm Hill` | Not in (h:)mm:ss format | 11 |
| 1 | FinishTime | `Irvine Running Club` | Not in (h:)mm:ss format | 103 |
| 1 | FinishTime | `Lochtayside` | Not in (h:)mm:ss format | 63 |
| 3 | FinishTime | `Lomond Hill Runners` | Not in (h:)mm:ss format | 45, 66, 94 |
| 10 | FinishTime | `Lothian` | Not in (h:)mm:ss format | 24, 30, 37, 41, 64, 67, 71, 77, 82, 92 |
| 1 | FinishTime | `Millburn Harriers` | Not in (h:)mm:ss format | 47 |
| 1 | FinishTime | `Moorfoots` | Not in (h:)mm:ss format | 14 |
| 1 | FinishTime | `Newcastle AC` | Not in (h:)mm:ss format | 48 |
| 4 | FinishTime | `Ochils` | Not in (h:)mm:ss format | 16, 32, 44, 50 |
| 5 | FinishTime | `Penicuik` | Not in (h:)mm:ss format | 65, 78, 80, 81, 90 |
| 1 | FinishTime | `Rochdale Harriers` | Not in (h:)mm:ss format | 68 |
| 1 | FinishTime | `Run4it-Edinburgh` | Not in (h:)mm:ss format | 79 |
| 1 | FinishTime | `Teviotdale` | Not in (h:)mm:ss format | 93 |
| 1 | FinishTime | `Tinto` | Not in (h:)mm:ss format | 87 |
| 7 | FinishTime | `U/A` | Not in (h:)mm:ss format | 29, 59, 69, 83, 85, 91, 97 |
| 9 | FinishTime | `Westerlands` | Not in (h:)mm:ss format | 6, 49, 60, 73, 86, 95, 100, 101, 102 |

## `races/Chapelgill/2025.csv`

**Row issues (1 unique, 3 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 3 | RunnerCategory | `60` | Invalid; cannot normalise to [MFN](dd)? | 43, 44, 49 |

## `races/Cornalees/2023.csv`

**Header issues:**

- Non-standard column name `FinishPosition` (expected `RunnerPosition`)

## `races/CraigDunain/2010.csv`

**Row issues (9 unique, 9 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | RunnerCategory | `F1` | Invalid; cannot normalise to [MFN](dd)? | 24 |
| 1 | RunnerCategory | `F2` | Invalid; cannot normalise to [MFN](dd)? | 25 |
| 1 | RunnerCategory | `F3` | Invalid; cannot normalise to [MFN](dd)? | 34 |
| 1 | RunnerCategory | `M1` | Invalid; cannot normalise to [MFN](dd)? | 2 |
| 1 | RunnerCategory | `M2` | Invalid; cannot normalise to [MFN](dd)? | 3 |
| 1 | RunnerCategory | `M3` | Invalid; cannot normalise to [MFN](dd)? | 4 |
| 1 | RunnerCategory | `MV1` | Invalid; cannot normalise to [MFN](dd)? | 5 |
| 1 | RunnerCategory | `MV2` | Invalid; cannot normalise to [MFN](dd)? | 6 |
| 1 | RunnerCategory | `MV3` | Invalid; cannot normalise to [MFN](dd)? | 8 |

## `races/CreagDhubh/2012.csv`

**Row issues (1 unique, 1 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | RunnerCategory | `???` | Invalid; cannot normalise to [MFN](dd)? | 51 |

## `races/Criffel/2015.csv`

**Row issues (1 unique, 2 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 2 | RunnerCategory | `Sweeper` | Invalid; cannot normalise to [MFN](dd)? | 50, 52 |

## `races/DeucharyHillCanter/2012.csv`

**Row issues (1 unique, 2 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 2 | RunnerCategory | `?` | Invalid; cannot normalise to [MFN](dd)? | 44, 45 |

## `races/DevilsBeeftub/2021.csv`

**Header issues:**

- Non-standard column name `FinishPosition` (expected `RunnerPosition`)

## `races/Dollar/2006.csv`

**Row issues (1 unique, 2 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 2 | RunnerCategory | `MSV60+` | Invalid; cannot normalise to [MFN](dd)? | 49, 181 |

## `races/Dumyat/2006.csv`

**Row issues (3 unique, 16 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 7 | RunnerCategory | `FUniv` | Invalid; cannot normalise to [MFN](dd)? | 143, 165, 183, 191, 194, 195, 199 |
| 7 | RunnerCategory | `MUniv40` | Invalid; cannot normalise to [MFN](dd)? | 77, 86, 99, 105, 154, 156, 158 |
| 2 | RunnerCategory | `MUniv50` | Invalid; cannot normalise to [MFN](dd)? | 67, 144 |

## `races/DurrisMast/2008.csv`

**Row issues (1 unique, 1 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | RunnerCategory | `Guest` | Invalid; cannot normalise to [MFN](dd)? | 11 |

## `races/Eildons/2021.csv`

**Header issues:**

- Non-standard column name `FinishPosition` (expected `RunnerPosition`)

## `races/Eildons/2022.csv`

**Header issues:**

- Non-standard column name `FinishPosition` (expected `RunnerPosition`)

## `races/Eildons/2023.csv`

**Header issues:**

- Non-standard column name `FinishPosition` (expected `RunnerPosition`)

## `races/El-Brim-IckDash/2013.csv`

**Row issues (1 unique, 1 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | RunnerCategory | `VIN` | Invalid; cannot normalise to [MFN](dd)? | 53 |

## `races/FalklandHillRace/2007.csv`

**Row issues (5 unique, 6 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | RunnerCategory | `FJ U11` | Invalid; cannot normalise to [MFN](dd)? | 36 |
| 1 | RunnerCategory | `FJ U12` | Invalid; cannot normalise to [MFN](dd)? | 37 |
| 2 | RunnerCategory | `FJ U13` | Invalid; cannot normalise to [MFN](dd)? | 21, 26 |
| 1 | RunnerCategory | `FJ U14` | Invalid; cannot normalise to [MFN](dd)? | 51 |
| 1 | RunnerCategory | `MJ U9` | Invalid; cannot normalise to [MFN](dd)? | 45 |

## `races/FalklandHillRace/2008.csv`

**Row issues (1 unique, 1 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | FinishTime | `late start` | Not in (h:)mm:ss format | 55 |

## `races/FalklandHillRace/2009.csv`

**Row issues (2 unique, 2 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | RunnerCategory | `FM60` | Invalid; cannot normalise to [MFN](dd)? | 34 |
| 1 | RunnerCategory | `M540` | Invalid; cannot normalise to [MFN](dd)? | 29 |

## `races/FalklandHillRace/2013.csv`

**Row issues (3 unique, 7 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 4 | RunnerCategory | `Ls` | Invalid; cannot normalise to [MFN](dd)? | 14, 29, 64, 74 |
| 2 | RunnerCategory | `Lu15` | Invalid; cannot normalise to [MFN](dd)? | 71, 75 |
| 1 | RunnerCategory | `Lu17` | Invalid; cannot normalise to [MFN](dd)? | 62 |

## `races/FalklandHillRace/2014.csv`

**Row issues (2 unique, 3 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 2 | RunnerCategory | `L40` | Invalid; cannot normalise to [MFN](dd)? | 23, 27 |
| 1 | RunnerCategory | `L50` | Invalid; cannot normalise to [MFN](dd)? | 21 |

## `races/FalklandHillRace/2015.csv`

**Row issues (2 unique, 2 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | RunnerCategory | `FJ U17` | Invalid; cannot normalise to [MFN](dd)? | 51 |
| 1 | RunnerCategory | `FJ U20` | Invalid; cannot normalise to [MFN](dd)? | 38 |

## `races/FalklandYomp/2022.csv`

**Header issues:**

- Non-standard column name `FinishPosition` (expected `RunnerPosition`)

## `races/FalklandYomp/2026.csv`

**Row issues (1 unique, 1 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | FinishTime | `0054:44` | Not in (h:)mm:ss format | 13 |

## `races/FetteressoForestMarathon/2023.csv`

**Row issues (1 unique, 1 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | RunnerCategory | `NB50` | Invalid; cannot normalise to [MFN](dd)? | 40 |

## `races/Glamaig/2006.csv`

**Row issues (3 unique, 3 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | RunnerCategory | `MHV` | Invalid; cannot normalise to [MFN](dd)? | 39 |
| 1 | RunnerCategory | `MS (L)` | Invalid; cannot normalise to [MFN](dd)? | 66 |
| 1 | RunnerCategory | `MV (L)` | Invalid; cannot normalise to [MFN](dd)? | 55 |

## `races/Glamaig/2007.csv`

**Row issues (1 unique, 2 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 2 | FinishTime | `M` | Not in (h:)mm:ss format | 68, 69 |

## `races/Glamaig/2008.csv`

**Row issues (1 unique, 1 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | FinishTime | `?` | Not in (h:)mm:ss format | 83 |

## `races/GlasTulaicheanUphill/2007.csv`

**Row issues (2 unique, 2 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | RunnerCategory | `F0` | Invalid; cannot normalise to [MFN](dd)? | 44 |
| 1 | RunnerCategory | `MM40` | Invalid; cannot normalise to [MFN](dd)? | 7 |

## `races/GreatWildernessChallenge/2022.csv`

**Header issues:**

- Non-standard column name `FinishPosition` (expected `RunnerPosition`)

## `races/GreatWildernessChallenge/2023.csv`

**Header issues:**

- Non-standard column name `FinishPosition` (expected `RunnerPosition`)

## `races/GypsyGlen/2008.csv`

**Row issues (1 unique, 1 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | RunnerCategory | `F3` | Invalid; cannot normalise to [MFN](dd)? | 27 |

## `races/GypsyGlen/2010.csv`

**Row issues (9 unique, 9 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | RunnerCategory | `F1, FV1` | Invalid; cannot normalise to [MFN](dd)? | 16 |
| 1 | RunnerCategory | `F2` | Invalid; cannot normalise to [MFN](dd)? | 18 |
| 1 | RunnerCategory | `F3, FV2` | Invalid; cannot normalise to [MFN](dd)? | 22 |
| 1 | RunnerCategory | `FV3` | Invalid; cannot normalise to [MFN](dd)? | 43 |
| 1 | RunnerCategory | `M1, MV1` | Invalid; cannot normalise to [MFN](dd)? | 2 |
| 1 | RunnerCategory | `M2` | Invalid; cannot normalise to [MFN](dd)? | 3 |
| 1 | RunnerCategory | `M3` | Invalid; cannot normalise to [MFN](dd)? | 4 |
| 1 | RunnerCategory | `MV2` | Invalid; cannot normalise to [MFN](dd)? | 5 |
| 1 | RunnerCategory | `MV3` | Invalid; cannot normalise to [MFN](dd)? | 9 |

## `races/HalfNevis/2007.csv`

**Row issues (1 unique, 1 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | RunnerCategory | `F(u20)` | Invalid; cannot normalise to [MFN](dd)? | 42 |

## `races/HalfNevis/2011.csv`

**Row issues (2 unique, 2 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | RunnerCategory | `Junior Man` | Invalid; cannot normalise to [MFN](dd)? | 41 |
| 1 | RunnerCategory | `female Vet 60 +` | Invalid; cannot normalise to [MFN](dd)? | 56 |

## `races/HuntersBogTrot/2007.csv`

**Row issues (1 unique, 7 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 7 | RunnerCategory | `SV60+` | Invalid; cannot normalise to [MFN](dd)? | 41, 58, 71, 75, 77, 80, 81 |

## `races/HuntersBogTrot/2009.csv`

**Row issues (2 unique, 4 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 2 | RunnerCategory | `F Jnr` | Invalid; cannot normalise to [MFN](dd)? | 57, 75 |
| 2 | RunnerCategory | `M Jnr` | Invalid; cannot normalise to [MFN](dd)? | 10, 11 |

## `races/HuntersBogTrot/2013.csv`

**Row issues (2 unique, 3 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | RunnerCategory | `FJnr - Student` | Invalid; cannot normalise to [MFN](dd)? | 110 |
| 2 | RunnerCategory | `MJnr - Student` | Invalid; cannot normalise to [MFN](dd)? | 10, 11 |

## `races/HuntersBogTrot/2019.csv`

**Row issues (1 unique, 1 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | RunnerCategory | `T50` | Invalid; cannot normalise to [MFN](dd)? | 94 |

## `races/KillinGames/2010.csv`

**Row issues (1 unique, 2 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 2 | RunnerCategory | `F Under 30` | Invalid; cannot normalise to [MFN](dd)? | 46, 48 |

## `races/KillinGames/2011.csv`

**Row issues (1 unique, 1 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | RunnerCategory | `M Over 65` | Invalid; cannot normalise to [MFN](dd)? | 21 |

## `races/KilpatricksCaper/2006.csv`

**Row issues (3 unique, 6 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 3 | RunnerCategory | `LVet 40` | Invalid; cannot normalise to [MFN](dd)? | 25, 51, 53 |
| 2 | RunnerCategory | `LVet 50` | Invalid; cannot normalise to [MFN](dd)? | 47, 52 |
| 1 | RunnerCategory | `Lvet 40` | Invalid; cannot normalise to [MFN](dd)? | 43 |

## `races/KilpatricksCaper/2007.csv`

**Row issues (2 unique, 4 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 2 | RunnerCategory | `Vet 40 L` | Invalid; cannot normalise to [MFN](dd)? | 42, 62 |
| 2 | RunnerCategory | `Vet 50 L` | Invalid; cannot normalise to [MFN](dd)? | 58, 59 |

## `races/Kinnoull/2009.csv`

**Row issues (1 unique, 1 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | RunnerCategory | `FVS` | Invalid; cannot normalise to [MFN](dd)? | 95 |

## `races/Kinnoull/2010.csv`

**Row issues (2 unique, 3 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 2 | RunnerCategory | `FVS` | Invalid; cannot normalise to [MFN](dd)? | 108, 118 |
| 1 | RunnerCategory | `MVS` | Invalid; cannot normalise to [MFN](dd)? | 93 |

## `races/Knockfarrel/2025.csv`

**Row issues (1 unique, 7 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 7 | RunnerCategory | `OSEN` | Invalid; cannot normalise to [MFN](dd)? | 3, 4, 8, 17, 24, 28, 35 |

## `races/Krunce/2023-1.csv`

**Header issues:**

- Non-standard column name `FinishPosition` (expected `RunnerPosition`)

## `races/Krunce/2023-2.csv`

**Header issues:**

- Non-standard column name `FinishPosition` (expected `RunnerPosition`)

## `races/Krunce/2023-3.csv`

**Header issues:**

- Non-standard column name `FinishPosition` (expected `RunnerPosition`)

## `races/Krunce/2023-4.csv`

**Header issues:**

- Non-standard column name `FinishPosition` (expected `RunnerPosition`)

## `races/LairigGhru/2010.csv`

**Row issues (1 unique, 1 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | RunnerCategory | `?FV` | Invalid; cannot normalise to [MFN](dd)? | 46 |

## `races/LomondsOfFife/2008.csv`

**Row issues (1 unique, 1 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | RunnerCategory | `M Vold` | Invalid; cannot normalise to [MFN](dd)? | 65 |

## `races/MaddyMoss/2021.csv`

**Header issues:**

- Non-standard column name `FinishPosition` (expected `RunnerPosition`)

## `races/Meall-aBhuachaille/2010.csv`

**Row issues (1 unique, 2 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 2 | RunnerCategory | `MF40` | Invalid; cannot normalise to [MFN](dd)? | 97, 115 |

## `races/Meall-aBhuachaille/2013.csv`

**Row issues (1 unique, 1 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | RunnerCategory | `LAC` | Invalid; cannot normalise to [MFN](dd)? | 121 |

## `races/Meall-nanTarmachan/2011.csv`

**Row issues (1 unique, 2 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 2 | RunnerCategory | `M Over 65` | Invalid; cannot normalise to [MFN](dd)? | 46, 59 |

## `races/Melantee/2007.csv`

**Row issues (1 unique, 1 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | RunnerCategory | `F(u20)` | Invalid; cannot normalise to [MFN](dd)? | 28 |

## `races/MitherTap/2013.csv`

**Row issues (1 unique, 1 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | RunnerCategory | `MA` | Invalid; cannot normalise to [MFN](dd)? | 15 |

## `races/MitherTap/2015.csv`

**Row issues (2 unique, 3 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | RunnerCategory | `FUV` | Invalid; cannot normalise to [MFN](dd)? | 61 |
| 2 | RunnerCategory | `MUV` | Invalid; cannot normalise to [MFN](dd)? | 41, 49 |

## `races/MoffatChase/2006.csv`

**Row issues (1 unique, 2 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 2 | RunnerCategory | `L40` | Invalid; cannot normalise to [MFN](dd)? | 61, 71 |

## `races/Morven/2009.csv`

**Row issues (1 unique, 2 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 2 | RunnerCategory | `MHV` | Invalid; cannot normalise to [MFN](dd)? | 35, 37 |

## `races/NormansLaw/2006.csv`

**Row issues (3 unique, 4 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | RunnerCategory | `FJ U13` | Invalid; cannot normalise to [MFN](dd)? | 73 |
| 2 | RunnerCategory | `FJ U17` | Invalid; cannot normalise to [MFN](dd)? | 61, 71 |
| 1 | RunnerCategory | `FJ U18` | Invalid; cannot normalise to [MFN](dd)? | 66 |

## `races/NormansLaw/2007.csv`

**Row issues (3 unique, 3 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | RunnerCategory | `FJ U13` | Invalid; cannot normalise to [MFN](dd)? | 51 |
| 1 | RunnerCategory | `FJ U20` | Invalid; cannot normalise to [MFN](dd)? | 83 |
| 1 | RunnerCategory | `Unatt.` | Invalid; cannot normalise to [MFN](dd)? | 55 |

## `races/NormansLaw/2011.csv`

**Row issues (1 unique, 1 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | RunnerCategory | `FJ U17` | Invalid; cannot normalise to [MFN](dd)? | 33 |

## `races/NorthBerwickLaw/2007.csv`

**Row issues (1 unique, 1 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | RunnerCategory | `10B` | Invalid; cannot normalise to [MFN](dd)? | 188 |

## `races/NorthBerwickLaw/2010.csv`

**Row issues (2 unique, 3 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 2 | RunnerCategory | `M.` | Invalid; cannot normalise to [MFN](dd)? | 102, 104 |
| 1 | RunnerCategory | `M. O40` | Invalid; cannot normalise to [MFN](dd)? | 40 |

## `races/NorthBerwickLaw/2012.csv`

**Row issues (12 unique, 30 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 2 | RunnerCategory | `B(10)` | Invalid; cannot normalise to [MFN](dd)? | 156, 158 |
| 2 | RunnerCategory | `B(11)` | Invalid; cannot normalise to [MFN](dd)? | 105, 184 |
| 6 | RunnerCategory | `B(13)` | Invalid; cannot normalise to [MFN](dd)? | 26, 62, 70, 100, 140, 147 |
| 5 | RunnerCategory | `B(14)` | Invalid; cannot normalise to [MFN](dd)? | 90, 133, 167, 204, 209 |
| 3 | RunnerCategory | `B(15)` | Invalid; cannot normalise to [MFN](dd)? | 47, 56, 145 |
| 1 | RunnerCategory | `B915)` | Invalid; cannot normalise to [MFN](dd)? | 69 |
| 1 | RunnerCategory | `G(10)` | Invalid; cannot normalise to [MFN](dd)? | 205 |
| 3 | RunnerCategory | `G(12)` | Invalid; cannot normalise to [MFN](dd)? | 172, 177, 201 |
| 1 | RunnerCategory | `G(13)` | Invalid; cannot normalise to [MFN](dd)? | 211 |
| 2 | RunnerCategory | `G(14)` | Invalid; cannot normalise to [MFN](dd)? | 77, 134 |
| 3 | RunnerCategory | `G(15)` | Invalid; cannot normalise to [MFN](dd)? | 148, 162, 210 |
| 1 | RunnerCategory | `X` | Invalid; cannot normalise to [MFN](dd)? | 102 |

## `races/RedMossKilps/2021.csv`

**Row issues (2 unique, 9 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 3 | RunnerCategory | `WU21` | Invalid; cannot normalise to [MFN](dd)? | 49, 71, 113 |
| 6 | RunnerCategory | `WU23` | Invalid; cannot normalise to [MFN](dd)? | 58, 60, 62, 63, 78, 126 |

## `races/RedMossRevolution/2007.csv`

**Row issues (1 unique, 5 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 5 | RunnerCategory | `L40` | Invalid; cannot normalise to [MFN](dd)? | 49, 64, 68, 78, 79 |

## `races/RedMossRevolution/2008.csv`

**Row issues (1 unique, 2 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 2 | RunnerCategory | `LU23` | Invalid; cannot normalise to [MFN](dd)? | 11, 80 |

## `races/Saughhill/2008.csv`

**Row issues (4 unique, 8 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | RunnerCategory | `Male U/12` | Invalid; cannot normalise to [MFN](dd)? | 27 |
| 3 | RunnerCategory | `Male U/14` | Invalid; cannot normalise to [MFN](dd)? | 14, 26, 30 |
| 1 | RunnerCategory | `Male U/16` | Invalid; cannot normalise to [MFN](dd)? | 8 |
| 3 | RunnerCategory | `Male U/18` | Invalid; cannot normalise to [MFN](dd)? | 4, 6, 17 |

## `races/Saughhill/2012.csv`

**Row issues (1 unique, 1 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | RunnerCategory | `Male (age 14)` | Invalid; cannot normalise to [MFN](dd)? | 3 |

## `races/Saughhill/2016.csv`

**Row issues (5 unique, 10 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 3 | RunnerCategory | `J F U 14` | Invalid; cannot normalise to [MFN](dd)? | 9, 18, 23 |
| 1 | RunnerCategory | `J F U 17` | Invalid; cannot normalise to [MFN](dd)? | 4 |
| 1 | RunnerCategory | `J M U 12` | Invalid; cannot normalise to [MFN](dd)? | 33 |
| 3 | RunnerCategory | `J M U 14` | Invalid; cannot normalise to [MFN](dd)? | 8, 16, 28 |
| 2 | RunnerCategory | `J M U 16` | Invalid; cannot normalise to [MFN](dd)? | 2, 14 |

## `races/Screel/2008.csv`

**Row issues (1 unique, 2 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 2 | RunnerCategory | `MV60+` | Invalid; cannot normalise to [MFN](dd)? | 29, 38 |

## `races/SnowRunningGlenshee/2024.csv`

**Row issues (1 unique, 3 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 3 | RunnerCategory | `Junior (18-20)` | Invalid; cannot normalise to [MFN](dd)? | 8, 13, 46 |

## `races/Tap-oNoth/2006.csv`

**Row issues (1 unique, 5 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 5 | RunnerCategory | `SVet` | Invalid; cannot normalise to [MFN](dd)? | 25, 29, 35, 40, 43 |

## `races/Tap-oNoth/2007.csv`

**Row issues (1 unique, 5 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 5 | RunnerCategory | `N/A` | Invalid; cannot normalise to [MFN](dd)? | 2, 14, 19, 20, 22 |

## `races/Tap-oNoth/2008.csv`

**Row issues (1 unique, 1 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | RunnerCategory | `FV Eq Rec` | Invalid; cannot normalise to [MFN](dd)? | 17 |

## `races/TaynuiltGames/2018.csv`

**Row issues (2 unique, 2 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | FinishTime | `M` | Not in (h:)mm:ss format | 2 |
| 1 | RunnerCategory | `USA"` | Invalid; cannot normalise to [MFN](dd)? | 2 |

## `races/Tinto/1994.csv`

**Row issues (1 unique, 1 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | FinishTime | `?` | Not in (h:)mm:ss format | 131 |

## `races/Tinto/1997.csv`

**Row issues (1 unique, 1 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | RunnerCategory | `SSSV` | Invalid; cannot normalise to [MFN](dd)? | 92 |

## `races/Tinto/1998.csv`

**Row issues (1 unique, 1 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | FinishTime | `?` | Not in (h:)mm:ss format | 49 |

## `races/Tinto/2000.csv`

**Row issues (1 unique, 2 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 2 | RunnerPosition | `78=` | Not a positive integer | 79, 80 |

## `races/Tinto/2001.csv`

**Row issues (5 unique, 15 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | RunnerCategory | `Jnr` | Invalid; cannot normalise to [MFN](dd)? | 29 |
| 5 | RunnerCategory | `L/S` | Invalid; cannot normalise to [MFN](dd)? | 93, 97, 102, 105, 119 |
| 2 | RunnerCategory | `L/Vet` | Invalid; cannot normalise to [MFN](dd)? | 118, 120 |
| 2 | RunnerCategory | `Over60` | Invalid; cannot normalise to [MFN](dd)? | 107, 108 |
| 5 | RunnerCategory | `S/L` | Invalid; cannot normalise to [MFN](dd)? | 50, 59, 65, 68, 112 |

## `races/Tinto/2003.csv`

**Row issues (3 unique, 5 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | RunnerCategory | `FDS` | Invalid; cannot normalise to [MFN](dd)? | 147 |
| 1 | RunnerCategory | `SSSV` | Invalid; cannot normalise to [MFN](dd)? | 97 |
| 3 | RunnerCategory | `VS` | Invalid; cannot normalise to [MFN](dd)? | 103, 128, 129 |

## `races/Tinto/2004.csv`

**Row issues (1 unique, 1 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | RunnerCategory | `JNR` | Invalid; cannot normalise to [MFN](dd)? | 108 |

## `races/Tinto/2017.csv`

**Row issues (2 unique, 2 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | FinishTime | `F50` | Not in (h:)mm:ss format | 143 |
| 1 | RunnerCategory | `HBT` | Invalid; cannot normalise to [MFN](dd)? | 143 |

## `races/Tom-naBat/2007.csv`

**Row issues (1 unique, 11 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 11 | FinishTime | `NULL` | Not in (h:)mm:ss format | 5, 9, 10, 11, 12, 13, 16, 17, 18, 19, … (+1) |

## `races/Turnhouse/2009.csv`

**Row issues (1 unique, 1 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | RunnerCategory | `NV40` | Invalid; cannot normalise to [MFN](dd)? | 71 |

## `races/TwoBreweries/1991.csv`

**Header issues:**

- Extra column `Year` — each year's results should be in its own file
- Non-standard column name `Pos` (expected `RunnerPosition`)
- Non-standard column name `Cat` (expected `RunnerCategory`)
- Non-standard column name `Time` (expected `FinishTime`)

## `races/TwoBreweries/1993.csv`

**Header issues:**

- Extra column `Year` — each year's results should be in its own file
- Non-standard column name `Pos` (expected `RunnerPosition`)
- Non-standard column name `Cat` (expected `RunnerCategory`)
- Non-standard column name `Time` (expected `FinishTime`)

## `races/TwoBreweries/1995.csv`

**Header issues:**

- Extra column `Year` — each year's results should be in its own file
- Non-standard column name `Pos` (expected `RunnerPosition`)
- Non-standard column name `Cat` (expected `RunnerCategory`)
- Non-standard column name `Time` (expected `FinishTime`)

## `races/TwoBreweries/1996.csv`

**Header issues:**

- Extra column `Year` — each year's results should be in its own file
- Non-standard column name `Pos` (expected `RunnerPosition`)
- Non-standard column name `Time` (expected `FinishTime`)
- Non-standard column name `Cat` (expected `RunnerCategory`)

## `races/TwoBreweries/1997.csv`

**Header issues:**

- Extra column `Year` — each year's results should be in its own file
- Non-standard column name `Pos` (expected `RunnerPosition`)
- Non-standard column name `Time` (expected `FinishTime`)
- Non-standard column name `Cat` (expected `RunnerCategory`)

## `races/TwoBreweries/1998.csv`

**Header issues:**

- Extra column `Year` — each year's results should be in its own file
- Non-standard column name `Pos` (expected `RunnerPosition`)
- Non-standard column name `Cat` (expected `RunnerCategory`)
- Non-standard column name `Time` (expected `FinishTime`)

## `races/TwoBreweries/1999.csv`

**Header issues:**

- Extra column `Year` — each year's results should be in its own file
- Non-standard column name `Pos` (expected `RunnerPosition`)
- Non-standard column name `Cat` (expected `RunnerCategory`)
- Non-standard column name `Time` (expected `FinishTime`)

## `races/TwoBreweries/2000.csv`

**Header issues:**

- Extra column `Year` — each year's results should be in its own file
- Non-standard column name `Pos` (expected `RunnerPosition`)
- Non-standard column name `Cat` (expected `RunnerCategory`)
- Non-standard column name `Time` (expected `FinishTime`)

## `races/TwoBreweries/2003.csv`

**Header issues:**

- Extra column `Year` — each year's results should be in its own file
- Non-standard column name `Pos` (expected `RunnerPosition`)
- Non-standard column name `Cat` (expected `RunnerCategory`)
- Non-standard column name `Time` (expected `FinishTime`)

## `races/TwoBreweries/2004.csv`

**Header issues:**

- Extra column `Year` — each year's results should be in its own file
- Non-standard column name `Pos` (expected `RunnerPosition`)
- Non-standard column name `Cat` (expected `RunnerCategory`)
- Non-standard column name `Time` (expected `FinishTime`)

## `races/TwoBreweries/2009.csv`

**Row issues (5 unique, 13 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | RunnerCategory | `FSNR L` | Invalid; cannot normalise to [MFN](dd)? | 69 |
| 5 | RunnerCategory | `MSNR L` | Invalid; cannot normalise to [MFN](dd)? | 8, 16, 43, 62, 72 |
| 2 | RunnerCategory | `MV40 L` | Invalid; cannot normalise to [MFN](dd)? | 51, 75 |
| 4 | RunnerCategory | `MV40L` | Invalid; cannot normalise to [MFN](dd)? | 21, 41, 61, 107 |
| 1 | RunnerCategory | `MV50 L` | Invalid; cannot normalise to [MFN](dd)? | 99 |

## `races/TwoBreweries/2012.csv`

**Row issues (1 unique, 1 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | RunnerCategory | `Under 20` | Invalid; cannot normalise to [MFN](dd)? | 25 |

## `races/TwoBreweries/2013.csv`

**Row issues (1 unique, 2 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 2 | RunnerCategory | `Junior 18+` | Invalid; cannot normalise to [MFN](dd)? | 7, 58 |

## `races/TwoBreweries/2024.csv`

**Row issues (1 unique, 1 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | RunnerCategory | `NB40` | Invalid; cannot normalise to [MFN](dd)? | 94 |

## `races/WhangieWhizz/2024.csv`

**Row issues (1 unique, 1 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 1 | RunnerCategory | `A` | Invalid; cannot normalise to [MFN](dd)? | 67 |

## `races/WhiteTops/2011.csv`

**Row issues (1 unique, 2 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 2 | RunnerCategory | `over 60` | Invalid; cannot normalise to [MFN](dd)? | 42, 47 |

## `races/Yetholm/2012.csv`

**Row issues (3 unique, 22 total):**

| Count | Column | Value | Issue | Rows |
|-------|--------|-------|-------|------|
| 8 | RunnerCategory | `Senior Ladies` | Invalid; cannot normalise to [MFN](dd)? | 15, 30, 37, 50, 58, 68, 78, 84 |
| 6 | RunnerCategory | `Veteran 40 Ladies` | Invalid; cannot normalise to [MFN](dd)? | 47, 65, 69, 76, 80, 87 |
| 8 | RunnerCategory | `Veteran 50 Ladies` | Invalid; cannot normalise to [MFN](dd)? | 49, 63, 67, 71, 73, 75, 79, 88 |

## `races/YetholmBordersShepherdsShow/2023.csv`

**Header issues:**

- Non-standard column name `FinishPosition` (expected `RunnerPosition`)

