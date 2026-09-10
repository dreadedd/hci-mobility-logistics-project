# Survey Analysis — University of Ghana Campus Mobility Survey

## Sample Overview

- **Respondents:** 35
- **Collection window:** 12–14 August 2026
- **Method:** Google Forms, distributed to University of Ghana students

### Level of Study

| Level | Count |
|---|---|
| Level 100 | 2 |
| Level 200 | 28 |
| Level 300 | 2 |
| Level 400 | 2 |
| Postgraduate | 1 |

The sample is heavily skewed toward Level 200 students (80%). Findings should be read as most representative of that group; Level 100/300/400 and postgraduate views are present but too few to generalise confidently.

### Frequency of Movement Around Campus (per day)

| Frequency | Count |
|---|---|
| Once | 4 |
| 2–3 times | 20 |
| 4–5 times | 7 |
| More than 5 times | 4 |

Most students (31/35, 89%) move around campus multiple times a day, confirming that mobility is a frequent, recurring task rather than an occasional one.

### Methods Commonly Used

| Method | Mentions |
|---|---|
| Walking | 26 |
| Taxi | 14 |
| Campus shuttle/bus | 8 |
| Personal vehicle | 5 |
| Ride-hailing app (Bolt/Uber/Yango) | 4 |
| Bicycle | 1 |

Walking and taxis dominate; the campus shuttle is used by less than a quarter of respondents, suggesting either low awareness, low reliability, or that it doesn't fit trip patterns.

### Ease of Finding Locations on Campus

| Rating | Count |
|---|---|
| Very easy | 8 |
| Easy | 8 |
| Neutral | 15 |
| Difficult | 3 |
| Very Difficult | 1 |

**30 of 35 (86%)** respondents said they have had difficulty finding a location on campus at some point, even though most rate general wayfinding as "Neutral" or better — i.e., wayfinding failures are occasional but widespread, not a constant struggle for most.

## Key Problems Reported (multi-select)

| Problem | Mentions |
|---|---|
| Difficulty finding buildings or lecture halls | 14 |
| Not knowing when a shuttle/bus will arrive | 12 |
| Difficulty finding transportation at certain times | 11 |
| Unclear pickup points | 8 |
| Long waiting times for transportation | 8 |
| Confusing routes | 5 |
| Other (free text) | 6 |
| Poor or insufficient campus signage | 2 |
| No problems experienced | 4 |

**The top two problem clusters are (1) wayfinding to buildings/lecture halls and (2) shuttle/transport unpredictability** (arrival times, pickup points, waiting times, availability at certain times) — together accounting for the large majority of complaints.

## How Students Currently Find Their Way

| Method | Count |
|---|---|
| Google Maps | 17 |
| Ask another student/person | 13 |
| Use a ride-hailing app | 2 |
| Call/message someone for directions | 2 |
| Follow campus signs | 1 |

Nearly 40% rely on asking another person rather than any digital tool — a strong signal that existing digital wayfinding (Google Maps, campus signage) does not fully meet on-campus navigation needs (e.g. building-level detail, indoor/lecture-hall precision).

## Most-Wanted Features (choose top 3)

| Feature | Mentions |
|---|---|
| Interactive campus map | 23 |
| Live shuttle/bus locations | 21 |
| Estimated shuttle arrival times | 16 |
| Directions to buildings and lecture halls | 15 |
| Pickup-point locations | 12 |
| Transport fares | 12 |
| Shuttle/bus route information | 9 |
| Accessibility information | 9 |
| Delay and service notifications | 8 |

**The four clear priorities are:** an interactive campus map, live shuttle tracking, estimated arrival times, and turn-by-turn directions to buildings/lecture halls. These directly map to the two problem clusters above.

## Recurring Themes in Open-Ended Responses

1. **Transport cost/fares** — the single most frequent frustration theme. Many respondents (≈10) singled out taxi/transport fares as "insane," "exorbitant," "painful," or charging the same rate regardless of distance. This is a strong candidate pain point even though it wasn't an explicit checkbox option in the problems question.
2. **Building/lecture hall wayfinding** — several respondents mentioned not being able to find lecture halls, confusing/abbreviated building names, and wanting building names reflected in navigation apps.
3. **Shuttle unpredictability** — not knowing when a shuttle will arrive, unclear pickup points, and requests for "live location of shuttles" and better shuttle timing.
4. **Campus scale/terrain** — a few mentions of the campus being large, having mountainous/hilly roads, and lacking shade while walking.
5. **A few "no problem" responses** — mostly non-resident students or students with lectures near one location, suggesting problem severity correlates with how spread out a student's daily routine is.

## Implications for Design Requirements

Based on this evidence, the following should be prioritised going into Requirements Definition (stage 4) and Wireframing (stage 5):

1. An **interactive campus map** with building/lecture-hall-level search and directions (addresses the top problem and top feature request).
2. **Live shuttle tracking with estimated arrival times** and clearly marked **pickup points** (addresses the second problem cluster).
3. Consider surfacing **transport fare information** for taxis/ride-hailing, given how dominant cost complaints were in open-text answers, even though it wasn't the top checkbox item.
4. Accessibility and delay/service notifications are lower-priority but still requested by roughly a quarter of respondents — worth including as secondary features.

## Interview Evidence (recalled post-hoc)

Photographic evidence of in-person interviews conducted with students on campus is available in `docs/02-user-research/interviews/` (4 photos, dated 2026-08-19). No notes were taken live during these interviews; the summary below was reconstructed afterward by the interviewers from memory (see `Interview_Recall_Worksheet.md` in the same folder) and should be read with that caveat — it is recalled, not recorded, evidence.

**Participants:** 3 separate Level 300 female students, interviewed on 19 August 2026 (afternoon, ~3–5pm) near the NNB car park. Interviewers: Obed Boateng Ayim, Emmanuella Ewurama Prah, Annabelle Naa Dedei Armah.

**Questions covered:** whether the timing of school shuttle arrivals is predictable, whether campus directions/navigation are clear, and whether an app showing live shuttle ETAs and accurate campus directions would be useful.

**Converging theme across all three interviews:**
- Shuttle arrival times were consistently described as unreliable, with no way to tell if a shuttle has been delayed or broken down en route — reinforcing the survey's #2/#3 most-common problems (shuttle unpredictability) and the #2 most-requested feature (live shuttle tracking).
- Existing map apps were described as having inaccurate or outdated campus building/direction data, reinforcing the survey's top problem (finding buildings/lecture halls) and top-requested feature (interactive campus map).
- On fares specifically, these three interviewees pushed back against the idea that an app needs dynamic pricing features — they described fares as fairly stable and said the main value would just be showing current prices, rather than anything more complex. This is a useful nuance against the survey's open-text finding that cost was the single most-mentioned frustration: it suggests the frustration may be more about the *price itself* being high, not that pricing is unclear or needs an in-app feature.
- One representative quote (paraphrased, not verbatim, and not attributed to a single named individual): students want **live tracking of shuttle locations on campus**, rather than a static estimated time.

**Interpretation caution:** all three interviewees were the same level and gender and were interviewed in the same location/time window, so this should be treated as one convergent snapshot rather than broad validation across the student population. It supports FR3/FR4 (live shuttle tracking, ETAs) and FR1/FR2 (interactive map, directions) but should not be used to deprioritise FR7 (fares) without further research, since only 3 (similar) students weighed in on that point.

## Limitations

- Sample is small (n=35 survey respondents) and skewed toward Level 200 students — not representative of the full student population.
- Self-selected respondents (Google Form) may over-represent students already frustrated with mobility issues.
- Interview evidence (n=3) was recalled from memory after the fact rather than recorded live, and all three interviewees shared similar demographics (Level 300, female) and were interviewed in the same session window — it corroborates the survey's top two problem areas but is not independent or broad validation, and should be weighted accordingly.
