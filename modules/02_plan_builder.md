> Change log: clarified how Module 2 selects activities. I added simple proximity rules, time blocks, pace-based duration, and default assumptions for missing info.

### **Module 2 — Plan Builder (Options → Days)**

Create a short list of candidate activities (e.g., attractions, restaurants, parks).  
Each activity must include minimal metadata:  
- **Duration** (short 1–2h, medium 2–3h, long 3–4h)  
- **Theme** (culture, nature, food, shopping, wellness, etc.)  
- **Cost band** ($ low, $$ mid, $$$ high)  
- **Distance band** (near ≤1 km / 15 min walk, moderate ≤3 km / 20 min transit)

Use basic time blocks to structure the day:  
- **Morning (09:00–12:00)**  
- **Midday (12:00–15:00)**  
- **Afternoon (15:00–18:00)**  
- **Evening (18:00–21:30)**

Reflect user pace when selecting activities:  
- **Relaxed:** 4–5h of activities plus meals/rest  
- **Balanced:** 6–7h of activities plus meals  
- **Fast:** 8–9h of activities plus meals/transit

Use a simple loop to build days:

for each day:  
- **Morning:** pick an activity near lodging (or city center if lodging is unknown).  
- **Midday:** pick an activity close by (near or moderate distance from morning).  
- **Afternoon:** pick an activity with a different theme; allow moderate transit.  
- **Evening:** always include a dinner option matching budget/diet; if adding an event, place dinner before or after within the evening block.

Default assumptions:  
- If lodging is unknown → anchor morning near the city center or main transit hub.  
- If budget is missing → default to mid-range ($$); if invalid or negative → clamp to low ($).  
- If time of year is unknown → include at least one indoor-capable option per day.