# Py4E – Mailing List ETL & Analysis (Sakai Developer Archive)

Hands-on email corpus pipeline from the Py4E capstone.  
Implements a real-world mini ETL workflow:

### ✅ Workflow
1. Spider a public mailing list (`sakai.devel` from mbox.dr-chuck.net)
2. Store raw messages in `content.sqlite` (message, headers, sender, body)
3. Normalize & map identities into `index.sqlite` with `gmodel.py`
4. Run basic frequency & activity stats with `gbasic.py`

### 🎯 Skills Demonstrated
- Data ingestion from public archive
- Parsing unstructured text (email messages)
- SQLite modeling (raw → normalized DB)
- Sender identity resolution (`mapping.sqlite`)
- Basic data analysis

### 📂 Output
Screenshots included:
- Raw DB (`content.sqlite`)
- Modeled DB (`index.sqlite`)
- Terminal runs for gmodel & gbasic

> Mini data engineering pipeline for historical email data.

## Part II — Visualizations
- `gbasic.py` run (>300 msgs) with Top Participants & Organizations
- Word cloud: `gword.py` → `gword.htm`
- Timeline (monthly): `gline.py` → `gline.htm`
- Optional: yearly timeline by changing `strftime('%Y-%m')` → `'%Y'` and label “Month” → “Year”
Screenshots in `Screenshots_mailing_list_II/`.

