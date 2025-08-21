# Budget Mapping Tool - Setup Instructions

Thank you for downloading the Budget Mapping Tool. https://mega.nz/file/bi5XRKLR#16ukqsqa-PwOhJmsE8iHRpCK7rRL7Dpg7uilcDnkvjU

## 1. Requirements
- Windows PC
- Excel with Macros enabled
- Python 3.9+ installed
- The Python package "xlwings" (for Excel ↔ Python connection)

## 2. Setup

1. Unzip this folder anywhere on your computer.
2. Open Command Prompt or PowerShell and navigate to the project folder.

   Example:
   `cd` "C:\Users\YourName\Desktop\BudgetMappingTool"

3. Install the required Python libraries:
   `pip install -r requirements.txt`

4. Install the xlwings Excel Add-in (only needed once per computer):
   `xlwings addin install`

## 3. Using the Tool

1. Open the Excel file: ***BudgetMapper.xlsm*** (present in folder BudgetMappingTool/excel)
2. Enable Macros when prompted.
3. Go to the **Settings** sheet:
   - Cell B2 → choose "US" or "CAD" for chart of accounts.
   - Cell B4 → set TRUE if you want to enable AI Notes (requires OpenAI key), otherwise leave FALSE.
4. Use the buttons on the Excel ribbon (added by xlwings) or in the workbook to:
   - Run Mapping
   - Review Exceptions
   - Apply Corrections
   - Export PDF

   Or click `Alt` + `F8`, then choose the task you want task (e.g. Run Mapping, Review Exceptions, etc.) and click `Run`.

## 4. Troubleshooting

- If you see "Sub or Function not defined":
  Make sure you installed the xlwings add-in (step 2.4).
- If Python scripts don’t run:
  Verify Python is installed and accessible from command line.
- If still facing any issue, ping me to get it resolved.

