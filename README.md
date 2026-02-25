# Friendly Squirrels? — Central Park Squirrel Census (2018)

**One-line hook:** I looked for the friendliest squirrels in Central Park — only about **6%** of sightings ever *approached* a human.  
**Project type:** Data story / beginner-friendly analysis (Python, Pandas, Matplotlib)

---

## Project question

**Which squirrels in Central Park are most likely to approach people, and what traits (fur color, age, location) do they share?**

---

## Dataset

- **Central Park Squirrel Census (2018)** — sightings CSV with ~3,023 records.  
  Source used: :contentReference[oaicite:0]{index=0} (dataset from :contentReference[oaicite:1]{index=1} / NYC Open Data).

---

## What I did (short)

1. Loaded the CSV and cleaned columns / duplicates.  
2. Converted boolean observation columns (`Running`, `Foraging`, `Approaches`, etc.) to `True/False`.  
3. Calculated summary stats (counts, approach rate).  
4. Visualized:
   - Fur color distribution
   - Activity counts (foraging, running, climbing,..)
   - Approach rate by fur color
   - (Optional) scatter map of sighting locations
5. Wrote a short story that highlights the surprise insight (the “Sherlock” moment).

---

## Key finding (TL;DR)
- **Only ≈ 5.9%** of sightings approached humans (i.e., friendly squirrels are rare).
- Cinnamon squirrels showed a higher approach *rate* vs their share of sightings — an interesting pattern to explore further.
- Most sightings are adults and most squirrels are gray by count, but color alone does not fully explain approach behaviour.

---

## Files in this repo
- `report.pdf` — final report / visuals (what I will submit to Codédex).  
- `squirrel_analysis.ipynb` — full Jupyter Notebook (code + charts + explanations).  
- `data/squirrels.csv` — source CSV (optional; include if the file size is small).  
- `outputs/` — generated images (`fur_color.png`, `activity_counts.png`, `approach_by_color.png`, ...).  
- `README.md` — this file.  
- `LICENSE` — project license (MIT).  
- `.gitignore` — recommended ignores.

---

## How to run (reproduce locally)
1. Clone the repo:
   ```bash
   git clone https://github.com/Hay0666/squirrel-data-story.git
   cd squirrel_project
