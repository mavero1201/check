# Prompt for AI Developer

Скопируй текст ниже целиком и отдай AI-разработчику.

---

Build a modern MVP web app called **Survey QA AI**.

## Product goal

The app must allow a user to upload a questionnaire document for a **quantitative marketing research survey** and receive an expert AI review of that questionnaire.

This is not a generic summarizer. The AI must act like a **senior quantitative marketing researcher** and audit the questionnaire professionally.

## Main user flow

1. User lands on a clean homepage.
2. User sees a drag-and-drop upload area.
3. User uploads a questionnaire document.
4. The app extracts text from the file.
5. The app sends the extracted text to an AI review module.
6. The app returns a structured report with findings and recommendations.

## File support

Support at least:
- PDF
- DOCX
- TXT

## UI requirements

Create a polished and minimal interface with:
- page title;
- short explanatory subtitle;
- drag-and-drop upload component;
- upload button fallback;
- loading state;
- processing state;
- error state;
- results page or results block.

Use a professional interface suitable for researchers and agency teams.

## AI review requirements

The AI review engine must check at minimum:

1. Duplicate answer codes.
2. Missing “Other” option when logically needed.
3. Missing “Don’t know / Hard to answer / No answer” option when methodologically needed.
4. Whether closed answer lists cover all realistic options.
5. Whether numeric or verbal ranges overlap.
6. Whether ranges leave gaps.
7. Whether the answer options truly answer the question.
8. Whether the question is leading, biased, double-barreled, overly complex, or assumes facts not in evidence.
9. Tone consistency, including consistent use of formal or informal address.
10. Standard quantitative questionnaire quality checks.

## Output format

The report must be structured by issue cards.
Each issue card should contain:
- category;
- severity (Critical / Major / Minor / Recommendation);
- problematic fragment;
- explanation;
- why it matters;
- recommendation.

Also add a summary section with total counts by severity.

## Technical preferences

Preferred stack:
- Next.js
- TypeScript
- Tailwind CSS
- Server-side API route for AI call

## Architecture expectations

Please create:
- a clean frontend structure;
- reusable upload component;
- parser utilities for file extraction;
- AI service layer;
- typed report model;
- mock mode or fallback sample result for local testing.

## Important logic

The app should be designed specifically for **quantitative survey questionnaire review**, not general document QA.

## Nice-to-have

- copy report button;
- downloadable report later;
- highlighted issue sections;
- simple sample questionnaire for testing.

## Deliverables

Generate a complete MVP codebase with:
- clear folder structure;
- setup instructions;
- environment variable example;
- clean UI;
- working upload and result flow.

---

Дополнительно передай AI-разработчику файлы `02_FUNCTIONAL_REQUIREMENTS.md`, `03_AI_REVIEW_RULES.md` и `05_ACCEPTANCE_CRITERIA.md` как часть контекста.
