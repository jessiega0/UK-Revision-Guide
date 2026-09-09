Life in the UK Revision Guide

ONLINE ACCESS

After GitHub Pages is enabled, open the revision guide in a web browser at:
https://jessiega0.github.io/UK-Revision-Guide/

OFFLINE ACCESS

1. Download the repository as a ZIP file using Code > Download ZIP on GitHub, or use a supplied ZIP copy.
2. Extract the ZIP file to a folder on your computer.
3. Open index.html in a web browser.

The revision guide works offline after extraction. Keep index.html, styles.css, and the assets folder together so that all images and fonts continue to load.

CSV REVISION HIGHLIGHTING

You can download or export question files from your Life in the UK source website and import them into the revision guide.

1. Select the Upload CSV button, shown as an upward arrow near the bottom-right corner.
2. Choose one or more files containing the questions you want to revise.
3. The guide compares the question text with its revision cards and marks matching cards with a red pill.

For the most reliable results, upload the CSV downloaded from the Life in the UK test website. Other CSV formats may not identify every question correctly.

The recommended table format is:

Question Number: Optional reference number.
Question: Required. The question to match against the revision cards.
Your Answer(s): Optional and ignored by the matcher.
Correct Answer(s): Recommended. Used to confirm the correct card when question wording differs.
Explanation: Optional and ignored by the matcher.

The importer accepts comma-separated CSV files as well as tab-, semicolon-, and pipe-separated files. It recognises question columns named Question, Question Text, Incorrect Question, Prompt, or Query. It recognises correct-answer columns named Correct Answer, Correct Answers, Correct Answer(s), or Expected Answer. A plain text file containing one question per line can also be used, but only exact or extremely close question matches are possible without a correct-answer column.

Matching first looks for the same question after ignoring capitalisation, punctuation, and repeated spaces. When wording differs, the correct answer can confirm one uniquely strong question match. Reversed question-and-answer wording is supported when both sides clearly agree. True, False, Yes, and No never provide positive matching evidence, and uncertain or ambiguous matches are not flagged.

CSV files are processed locally in your browser and are not uploaded to a server by this guide.

Red-pill revision selections are remembered in that browser until Reset is selected. The page viewpoint and expanded sections are remembered for 30 minutes; after that, the guide starts from its default view while keeping the red-pill selections.

WEBSITE CONTROLS

Expand: Opens all revision sections.
Collapse: Closes all revision sections.
Upload CSV: Opens the file picker and highlights cards matching questions in the selected files.
Search/Top: Returns to the top of the page and places the cursor in Search.
Take Quiz: Opens the Life in the UK quiz website in a new browser tab.

When revision cards are highlighted, the red-pill toolbar also appears:

Card count: Shows how many cards are highlighted for revision.
Focus mode: Hides sections and cards that are not part of the current revision selection.
Reset: Removes all imported red-pill revision selections from this browser.
Previous: Moves to the previous highlighted card.
Next: Moves to the next highlighted card.

OFFLINE ASSETS

All pictures and title fonts are included in the assets folder. No external image or font connection is required, so the complete guide can be used offline.
