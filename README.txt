THE REORDER ALARM
Build It With AI — Episode 11 giveaway

WHAT IT IS
A single HTML file. Open index.html in any browser (double click — no internet,
no account, nothing uploaded). Paste two exports from your point of sale:

  1. activity.csv — a year of rows: date, sku, item, type (SALE/RECEIVED), qty
  2. stock.csv — sku, item, on_hand, unit_cost, unit_price, pack_size,
     supplier, lead_time_days

It answers, for every item: reorder today / this week / OK / quiet / dead,
days of cover measured only against days the item was actually in stock,
a suggested order quantity rounded up to the supplier's pack, one purchase
order per supplier, the cash tied up in dead stock, and the revenue at risk
before new stock can arrive. Every row it refuses to use is listed with a
reason, and the footer reconciles opening + received − sold against your
stock file to the unit — or tells you not to trust the board.

SETTINGS (all visible in the tool)
  Velocity window (default 90 days) · Safety stock days (7)
  Dead after (180 days) · Order up to (14 extra days of cover)

FILES
  index.html                 the tool (this is the whole product)
  sample_activity.csv        a year of register activity for a fictional store
  sample_stock.csv           its stock file (all data fictional, @example.com class)
  PROMPTS.txt                the exact three prompts used on camera
  engine_v1_first_build.js   the first build, bugs and all (for the curious)
  checker.py                 the independent Python checker from the episode

NOTES
The sample business (Lantern Hardware Supply) is fictional. The tool proposes
orders; it does not place them. Nothing in this file talks to the internet.
