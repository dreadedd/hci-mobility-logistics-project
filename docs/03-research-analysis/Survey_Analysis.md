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

## Limitations

- Sample is small (n=35) and skewed toward Level 200 students — not representative of the full student population.
- Self-selected respondents (Google Form) may over-represent students already frustrated with mobility issues.
- No interview data yet — `docs/02-user-research/interviews/` is still empty. Interviews would help validate and deepen these survey findings before finalising requirements.
