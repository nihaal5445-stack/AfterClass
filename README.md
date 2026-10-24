# AfterClass

**Classes end. Learning shouldn't.**

AfterClass turns the last 10 minutes of a lecture into a short, optional check of what students understood. The professor asks one question about that day's class. Students who want to take part answer it. AI grades each answer against the professor's own notes, and every student gets feedback and a revision plan.

**Live demo:** https://nihaal5445-stack.github.io/AfterClass/

---

## The problem

- Many colleges give marks for attendance. Students come to class to be marked present, not always to learn.
- Most students revise only right before exams, so what they learn in class fades within days.
- Professors rarely have time to check how much of a lecture actually landed. A professor in our own department at NIT Warangal already asks surprise questions at the end of class, but checks every answer by hand.

## How AfterClass works

1. **Before class:** the professor uploads the notes for the lecture.
2. **End of class:** the professor posts one question about something that happened in that class, so a textbook or chatbot cannot answer it.
3. **Answer (optional):** students who wish to take part answer in their own words, in a timed window of about 10 minutes. No one is forced to write.
4. **AI grading:** each answer is checked against the professor's notes and key points. The student sees what they got right, what they missed, and short feedback.
5. **Revision plan:** every missed point becomes a revision card that comes back after 1, 3, 7 and 14 days.
6. **Bonus marks:** good answers earn points that add up to bonus marks, capped at full marks. Skipping never costs marks.
7. **Class summary:** the professor sees which points most students missed, so the next class can start there.
8. **Appeals:** a student who disagrees with a grade can appeal. The AI checks again first, then the professor decides.

## Try the demo

The demo walks through one real lecture (Database Systems, Lecture 14: Joins and indexes) in six steps.

1. **Before class:** look at the example notes, question and key points. You can change any of them.
2. Click **Post question to class**. A 10-minute timer starts.
3. Go to **Answer**. Write your own answer, or load a strong, weak or copied example, then click **Submit answer**.
4. **Result:** see your score, the points you covered and missed, and feedback. Try **Appeal this grade**.
5. **Revise:** see your revision cards and bonus total.
6. **Class summary:** see the most-missed points from the professor's side.

It works on a phone and a laptop.

## What is real in this demo and what is not

| Part | In this demo |
|---|---|
| Timer, answer window, closing the window | Working |
| Notes the student if they leave the screen while answering | Working |
| Flags answers that are almost the same as a classmate's | Working (compared with sample answers) |
| Grading | A simple key-point matcher that runs in the browser. In the full product, AI does this grading. |
| Revision cards and bonus total | Working for your answer; older cards are examples |
| Classmates' answers and class summary numbers | Example data, with your answer added in |
| Logins and saving data between classes | Not built yet |

## Planned build

- **Grading model:** GPT-4o mini, grading each answer against the professor's notes
- **Cost:** about ₹0.07 per answer, so a 300-student pilot over a full semester costs about ₹2,100 in AI fees
- **Speed:** a class of 60 answers graded in about a minute
- **Pilot budget:** about ₹20,000 in total (AI, hosting and domain)

## Built with

- One HTML file with plain HTML, CSS and JavaScript
- No frameworks, no build step, no server
- Hosted on GitHub Pages

To run it on your computer, download `index.html` and open it in any browser.

## Team AfterClass, NIT Warangal

| Name | Role |
|---|---|
| Nihal J N | Team lead |
| Afrid Basha | Team member |
| Neelam Jashwanth | Team member |

All three of us are B.Tech CSE students (3rd year) at NIT Warangal.

Built for the SEVA FIRST Innovation Challenge 2026.
