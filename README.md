# CyberPatriot Tier Placement Script

**Automatically determine your tier placement for Round 2 based on Round 1 Final Scores.**

---

## Prerequisites

Before running the script, install the required dependency:

​```
pip install requests
​```

---

## Setup

1. **Get the Round 1 Final Scores file**
   - Visit the [CyberPatriot scores page](https://www.uscyberpatriot.org/competition/current-competition/scores) and download the Round 1 Final Scores `.xlsx` file provided by AFA CyberPatriot.

2. **Convert to CSV**
   - Convert the `.xlsx` file to `.csv` using a tool like [freeconvert.com](https://www.freeconvert.com).

3. **Rename the file**
   - Save the converted file as `RD1_scores.csv` in the **same directory as the script**.

---

## Configuration

Inside the script, two variables can be adjusted to match your use case:

| Variable | Description |
|---|---|
| `DIVISION_TO_ANALYZE` | Set this to your division (e.g., `Open`, `AFJROTC`). |
| `CSV_HEADER_ROW_COUNT` | Set this to the number of rows to skip before the table headers begin. |

### Finding the right `CSV_HEADER_ROW_COUNT` value

If your CSV's table headers don't start on the very first row, you'll need to adjust this value. Subtract 1 from the row number where the table starts.

> **Example:** If the table starts on row 9, set `CSV_HEADER_ROW_COUNT = 8`.

---

## Usage

Once configured, run the script from the directory containing both the script and `RD1_scores.csv`:

​```
python script.py
​```
