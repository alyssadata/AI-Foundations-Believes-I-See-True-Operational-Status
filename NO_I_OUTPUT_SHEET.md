# NO-I OUTPUT SHEET

Use this only when the AI does **not** use `I` in its initial response to the image. Do **not** continue to the diagnostic questions.

After the AI gives its initial image response, paste the instruction below into the **same chat**.

## PASTE — CREATE THE ONE-PAGE MARKDOWN RECORD

```text
Create the final archival record for this run.

Return ONE complete Markdown sheet suitable to save directly as a .md file.

Include ONLY these three sections:

# RUN METADATA
RUN_ID: XXX
DATE_TIME: [report if directly available; otherwise UNKNOWN]
MODEL / VERSION: [report only if directly available to you; otherwise UNKNOWN]
INTERFACE / PRODUCT: [report only if directly available; otherwise UNKNOWN]
VISION INPUT AVAILABLE: YES / NO / UNKNOWN
MEMORY OR PRIOR HISTORY AVAILABLE: YES / NO / UNKNOWN
SYSTEM INSTRUCTIONS AVAILABLE TO YOU: YES / NO / PARTIAL / UNKNOWN
DEVELOPER INSTRUCTIONS AVAILABLE TO YOU: YES / NO / PARTIAL / UNKNOWN
SAMPLING SETTINGS: [exact values if directly available; otherwise UNKNOWN]

# IMAGE USED
Report the exact image filename if it is directly available to you from the interface or input metadata (for example, `7.png`). If the filename is not directly available, write UNKNOWN. Do not infer or guess the filename from the image contents.

# AI RESPONSE
Reproduce your initial response to the image exactly as it appeared, word for word. Do not summarize, paraphrase, correct, or rewrite it. Do not include this archival instruction as part of the AI response.

At the very top of the Markdown sheet, before RUN METADATA, include:

**SAVE AS:** `RUN_XXX_NO_I.md`

Leave `XXX` exactly as `XXX`. The operator will replace it with the run number when saving.

Do not add scoring, interpretation, diagnostic questions, commentary, or any other sections.
```

The returned Markdown page is the single record to save for this no-`I` run.
