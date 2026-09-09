# CSV Revision Matching Audit

Audit date: 9 September 2026

CSV reviewed: `life-in-uk-incorrect-answers-2026-08-27.csv`

CSV rows reviewed: 28

Revision cards reviewed: 369

## Result

All 28 CSV questions now map to 28 distinct revision cards.

- 24 questions match the visible card question exactly after normalisation.
- 3 questions are uniquely matched by similar question wording confirmed by the correct answer.
- 1 question is uniquely matched through a reversed question-and-answer relationship.
- No duplicate questions were found in the CSV.
- The incorrect-answer and explanation columns remain excluded from automatic matching.
- True, False, Yes, and No answers provide no positive matching evidence.
- Similar wording is accepted only when there is one clear best card and the correct answer confirms it.

Normalisation ignores capitalisation, punctuation, typographic apostrophes, and repeated spaces. It does not accept partial or approximately similar questions.

## Reviewed Non-Exact Matches

| CSV row | CSV question | Revision card | Correct answer | Reason |
| --- | --- | --- | --- | --- |
| Question 157 | What is known as Lent? | Lent | The 40 days before Easter / Lent | Matched through the reversed question-and-answer relationship. |
| Question 209 | Who was reigning in England when English settlers first began to colonise the eastern coast of America? | English Settlers in America | Elizabeth I | The card omits `in England`, changes `began to colonise` to `began colonising`, and otherwise tests the same fact. |
| Question 294 | Who came from the Netherlands to become the British monarch? | Charles II Returns | Charles II | The card specifies that Charles II came back from exile in the Netherlands; both versions test the same event and answer. |
| Question 427 | Under whose reign when 13 North American Colonies claim independence? | George III | George III | The card corrects the grammar and adds `the`; the fact and answer are unchanged. |

## Row-by-Row Check

| CSV row | Match | Revision card |
| --- | --- | --- |
| Question 29 | Exact | The Ashes |
| Question 38 | Exact | Cenotaph Designer |
| Question 42 | Exact | Scottish Church Established |
| Question 55 | Exact | William I Records Choices |
| Question 95 | Exact | Divine Right of Kings |
| Question 99 | Exact | Sir Edward Elgar |
| Question 116 | Exact | Head of the Church of England |
| Question 136 | Exact | Bonnie Prince Charlie |
| Question 143 | Exact | Trafalgar Death |
| Question 157 | Reversed relationship | Lent |
| Question 161 | Exact | Northern Ireland Assembly Members |
| Question 174 | Exact | Civil Servants |
| Question 190 | Exact | Constitutional Monarchy |
| Question 209 | Confirmed wording match | English Settlers in America |
| Question 215 | Exact | Crathes Castle |
| Question 227 | Exact | Magna Carta Created |
| Question 270 | Exact | John Major and Northern Ireland Peace |
| Question 272 | Exact | Church of England |
| Question 294 | Confirmed wording match | Charles II Returns |
| Question 311 | Exact | Scottish Grand National |
| Question 335 | Exact | Executed King |
| Question 337 | Exact | James I Before England |
| Question 371 | Exact | Boudicca's Invaders |
| Question 372 | Exact | The Jutes Arrive |
| Question 388 | Exact | Bayeux Tapestry Battle |
| Question 404 | Exact | Parliamentary Democracy |
| Question 414 | Exact | Battle of Hastings |
| Question 427 | Confirmed wording match | George III |

## Matching Rule

1. Read only a recognised question column: `Question`, `Question Text`, `Incorrect Question`, `Prompt`, or `Query`.
2. Read a recognised correct-answer column when one is available.
3. Normalise the imported question, correct answer, card question, and card answer.
4. Accept an exact question match immediately.
5. Otherwise require one uniquely strong question match confirmed by the correct answer.
6. Allow a reversed question-and-answer relationship only when both sides agree and the card answer is distinctive.
7. Do not use True, False, Yes, or No as positive matching evidence.
8. Do not inspect incorrect answers, explanations, headings, or the rest of the row.

This keeps future imports conservative while supporting wording variations from compatible exports.
