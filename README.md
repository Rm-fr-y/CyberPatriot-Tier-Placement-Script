# CyberPatriot-Tier-Placement-Script
For all of you that worry about your Tier placements during Round 2, this script will figure it out for you. \
Make sure that the Round 1 Final Scores CSV is saved with the filename of RD1_scores.csv.

To get the csv file you must - \
Convert the RD1 final scores xlsx file provided by AFA CyberPatriot at https://www.uscyberpatriot.org/competition/current-competition/scores to a csv. \
You can use a tool like freeconvert.com to achieve this. \
Rename the csv to RD1_scores.csv

Make sure to install the requirements and keep the Round 1 Final scores saved as a CSV in the same directory as the script. \
Command to install requirements: pip install requests

Within the script you may adjust the DIVISION_TO_ANALYZE and CSV_HEADER_ROW_COUNT variables based on your use case. \
The DIVISION_TO_ANALYZE variable is used to change the division you are in (Open, AFJROTC, etc.). \
The CSV_HEADER_ROW_COUNT is used to change where the script actually starts reading the csv. Depending on the way your csv is formatted, the table headers may not be on the first row. Utilize this variable to fix it, for example, if the table starts on the 9th row, you would skip 9-1=8 rows, and that would be your value for this variable.