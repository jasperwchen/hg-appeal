# HackGwinnett 6.0 Judge's Ranking

**Judge:** Claude Opus 5.5, xhigh effort
**Reviewed:** all 50 entries in `hackgwinnett-crawl.json`, against `HG-Prompt.md`
**Theme:** accessibility tools for navigating the medical care system for disabled users

## Top 10

Scores are out of 10 per criterion and 40 overall. P = practicality/relevance, C = creativity/innovation, S = significance, T = technical complexity.

| Rank | Project | What it does | P | C | S | T | Total |
|---|---|---|---|---|---|---|---|
| 1 | **AcuPath** (JabCross) | Spoken indoor hospital navigation for blind patients | 7.5 | 9.5 | 8.5 | 10 | **35.5** |
| 2 | **SMS Shield** | Medical, billing and legal rights help across several disabilities | 8.5 | 8 | 9 | 8.5 | **34** |
| 3 | **Pawthfinder** | Browser extension that guides users through patient portals | 7 | 9.5 | 8.5 | 8 | **33** |
| 4 | **HospitalRating** | Turns plain patient reviews into equipment-level accessibility data | 8 | 9 | 8 | 7.5 | **32.5** |
| 5 | **Clear Case** | Reshapes one medical document to fit each disability | 9 | 8 | 8 | 7 | **32** |
| 6 | **CareFit** | Matches access needs to clinics and drafts accommodation letters | 7.5 | 7.5 | 8.5 | 7.5 | **31** |
| 7 | **HealthLens** | Turns medical papers and pill photos into short, spoken steps | 9 | 6.5 | 7.5 | 8 | **31** |
| 8 | **Accessible Medical Care Navigator** | Offline-capable document simplifier with measured OCR | 8 | 7 | 7.5 | 8 | **30.5** |
| 9 | **Adaptive Touch** | iPhone interface that compensates for hand tremors | 6.5 | 9 | 7 | 8 | **30.5** |
| 10 | **AccessAhead** | Clinic finder that re-ranks by daily health and asks clinics for you | 7 | 8.5 | 8 | 5.5 | **29** |

AcuPath is the clear first place. The first nine projects also stay in the top 10 whichever criterion counts double, so the list doesn't depend on my equal weighting. Tenth place is the softest spot.

One check affects this list: confirm that SMS Shield meets the event's rules before announcing it. Details are under [Checks before announcing](#checks-before-announcing).

## How I judged

The prompt names four criteria but gives no weights, so each counts equally.

| Score | Practicality/relevance | Creativity/innovation | Significance | Technical complexity |
|---|---|---|---|---|
| 9-10 | A disabled patient could use it now, with no institution's help | A new approach that changes how the problem is framed | Removes a high-stakes barrier for many people | Several hard systems working together, with tests or evaluation |
| 7-8 | Works and is on-prompt, but needs real data, a partner or setup | A meaningful twist on a common pattern | High stakes for a defined group, or moderate stakes for many | Substantial full-stack or ML work showing engineering judgment |
| 5-6 | Partly works, with major gaps | A competent version of a common pattern | A real but moderate barrier | A working app built mostly from standard APIs or generated code |
| 3-4 | Tangential or barely functional | Little added | Narrow or low stakes | Simple |
| 1-2 | Off-prompt or unusable | None evident | Minimal | Trivial |

The same rules applied to every entry:

- **Same evidence:** I used only the crawl. I did not run any app, open any repo or watch any video, because visiting some links and not others would treat teams unequally.
- **Evidence over claims:** a feature earned credit when the writeup showed it existed. Roadmap items earned no credit. Contradictory claims earned partial credit at most.
- **Ignored factors:** team size, team names, personal stories, and which AI tools were used. AI-assisted coding was neither rewarded nor penalized, because the prompt doesn't address it.
- **Ties:** the project with the higher lowest score wins, since a project with no weak criterion is harder to dispute. Ties that survive this rule are listed in no particular order.

## Why each project placed where it did

### 1. AcuPath (`acupath`, called JabCross in its writeup)

**Strengths:** This is the only entry that takes on the physical hospital, where GPS stops working and directions are printed on signs. A chest-worn phone sends frames to a depth model, printed wall markers fix the patient's position, and a route graph drives spoken directions, with safety alerts taking priority. The engineering shows real judgment. The team fixed a 24% depth error, caught a covered lens that the model read as a wall, and added thresholds so the app speaks only when something changes. The navigator has 50 automated tests.

**Weaknesses:** It is not ready for patients. It needs printed markers, a mapped building and a laptop server. The hospital walkthrough in the video is a scripted simulation, which the team discloses, and no blind users have tested it. Bad guidance could injure someone, so it needs validation before any pilot.

**Placement:** It has the highest technical score and a joint-highest creativity score, and it stayed first whichever criterion counted double.

### 2. SMS Shield (`sms-shield-gtks0o`)

**Strengths:** This is the most complete tool in the field, with a public deployment. Its opening screen solves a problem most entries skip: how someone who can't see, hear or speak gets in before any settings exist. Each option lights up and is read aloud in turn, and one press selects it. It also offers head-tracked navigation in the browser, a shared legal layer with citations, six ready-to-send letters, and fallbacks when an outside service fails.

**Weaknesses:** Photo-based symptom checks carry medical risk even with careful wording. The commercial roadmap toward diagnostic hardware goes well past what has been validated. See the eligibility check below.

**Placement:** It is the most balanced entry, with no score under 8. AcuPath still leads, because its 3-point edge in creativity and technical work exceeds SMS Shield's 1.5-point edge in practicality and significance.

### 3. Pawthfinder (`pawthfinder-qagtbu`)

**Strengths:** A spoken goal such as "book a follow-up with my cardiologist" becomes guided steps across several portal pages. It warns about barriers ahead, such as mouse-only robot checks and phone-only steps, spots hidden sign-out timers, and saves the user's answers. It asks "what helps you?" instead of sorting people into disability categories, and it refuses to enter passwords or tick consent boxes. The team's AI test agents, acting as disabled users, found real problems such as keyboard focus being lost after closing a notice.

**Weaknesses:** It was tested only on the team's own mock portal. Understanding any real medical website is listed as future work, which is why practicality is 7.

**Placement:** It is the most inventive answer to the digital side of the prompt. It sits below SMS Shield because that project isn't limited to a mock site.

### 4. HospitalRating (`avaneesh-nelakosigi`, listed under the author's name)

**Strengths:** CareFit, AccessAhead, AccessReady and CareCost all run into the same wall: clinics don't publish equipment data. This entry built the most concrete way to produce it. Patients write ordinary reviews, and two Naive Bayes classifiers written from scratch sort each sentence by equipment and by whether it worked. Results appear beside what the hospital says, and below 60% confidence the app asks the user instead of guessing. It covers 23 real metro Atlanta and Gwinnett locations and marks anything unverified.

**Weaknesses:** It has a cold-start problem, because the reviews so far are labeled demo data. The accuracy figures also deserve caution. They fit about 32 held-out sentences, from a dataset written for the project. On that sample, the 81.3% worked/failed accuracy has a 95% range of roughly 65-91%.

**Placement:** It combines an original idea with honest measurement, and it is the most locally relevant entry in the top 10. It sits half a point behind Pawthfinder, which addresses a wider barrier.

### 5. Clear Case (`carebridge-nih7wr`, called CareBridge in its writeup)

**Strengths:** It is the best of about a dozen document tools, and it needs no cooperation from any hospital. One bill, denial or discharge note becomes short read-aloud chunks for blind users, a text-only version with a drafted message for Deaf users, single-step cards for cognitive disabilities, or a low-effort checklist for fatigue. Users can interrupt at any point, get an answer quoted from the document, and resume where they stopped. If the document doesn't say, the app says so.

**Weaknesses:** It reads single document images, with PDFs and multi-page files still to come. The team states it hasn't tested with disabled users. It has less engineering depth than the four projects above it.

**Placement:** It has the joint-highest practicality score and the sharpest design among the document tools. It ranks fifth because the ideas above it are more original or technically harder.

### 6. CareFit (`carefit`)

**Strengths:** Patients mark each access need as required or nice to have, and each clinic's score is explained as has, missing or unknown. A match can then become an accommodation letter citing Section 504 and the ADA. The AI assistant runs on a local model, so messages don't go to an outside AI company. The team reports testing with Playwright and axe.

**Weaknesses:** The clinics are about 20 fictional Oakland locations, so matching can't help a real patient yet, and nothing in the build produces real clinic data. The letter is the part that is useful today.

**Placement:** It is the best-built clinic matcher. It ties HealthLens on 31 and wins on the lowest-score rule (7.5 to 6.5).

### 7. HealthLens (`healthlens-q418rj`)

**Strengths:** It is deployed and works from a real photo. Discharge papers become plain steps sorted by urgency, with tap-to-define words, read-aloud and calendar export. Pill and bottle checks give dosing only when it is printed on the label, and they admit uncertainty. The team wrote 58 tests and enforces safety rules in code instead of trusting the model.

**Weaknesses:** The concept is the most common one in the field, which gives it the lowest creativity score in the top 10. Pill results aren't yet checked against a drug database, and a wrong identification could cause harm. Testing with real users is still on the roadmap.

**Placement:** It has the joint-highest practicality score and strong engineering discipline, but it loses the tie with CareFit.

### 8. Accessible Medical Care Navigator (`accessible-medical-care-navigator`)

**Strengths:** It has the most disciplined engineering among the document tools. When OCR found only about 43% of key phrases on phone photos, the team built an evaluation harness and tested fixes one at a time, keeping one conditional step and dropping another that backfired. It removes personal details, links each simplified section to the original, and answers "Not in this document" when it can't answer. The same code runs as a website, offline app, desktop app and Android app.

**Weaknesses:** The writeup gives no final OCR figure and excludes insurance and billing documents. The crawl has a video but no repo or live link.

**Placement:** It ties Adaptive Touch on 30.5 and wins on the lowest-score rule. It ranks below Clear Case and HealthLens because it covers less of the patient's task.

### 9. Adaptive Touch (`adaptive-touch`)

**Strengths:** No other entry makes tremor its main barrier. This native iPhone app uses Core Motion to move the interface in response to phone movement, and adds larger targets, touch tolerance and accidental-tap protection. The team worked through real sensor problems, including overreaction to tilt, by focusing on lateral acceleration with smoothing.

**Weaknesses:** It works only inside its own demo app, and running it requires Xcode and a connected iPhone. Applying it to other software is theoretical for now.

**Placement:** It has a joint-third creativity score and real device-level engineering. Its limited reach holds down practicality and significance.

### 10. AccessAhead (`accessahead`)

**Strengths:** It has the best product thinking among the clinic finders. A daily check-in re-ranks clinics by how the patient feels that day, which suits fluctuating conditions. "Ask for Me" contacts a clinic to fill in unknown details, which matters for people who can't easily phone. Every fact is marked verified or unknown, with its source and date.

**Weaknesses:** Most of the evidence is design work. The stack is listed as CSS, Figma, Python and SVG, and the writeup doesn't explain how "Ask for Me" reaches clinics or where verified data comes from.

**Placement:** This is the softest placement. Its ideas earn it the spot, but HealthBridge replaces it if technical complexity counts double.

## Closest calls

- **AcuPath vs. SMS Shield:** SMS Shield is more useful today and AcuPath is the bigger achievement. Equal weights favor AcuPath by 1.5 points.
- **CareFit vs. HealthLens:** This is an exact tie decided by the tie-break rule. A judge who values working on real documents today could reasonably swap them.
- **AccessAhead vs. HealthBridge, AccessMed and Cadence AI:** All four are within a point. AccessAhead has the stronger ideas, HealthBridge the clearer working code, and Cadence AI the most focused design.

## Just outside the top 10

- **11. HealthBridge:** It has a real extension with an axe-core scanner, reader view and form helper on live pages, but its AI features are left undescribed.
- **12. AccessMed:** It is a well-explained portal extension, but nothing shows it was tried on the real portals it names.
- **13. Cadence AI:** This is the most thoughtful design for one group, people with aphasia, including a way to say "that's not what I meant." It is a no-code prototype, which limits the technical score.
- **14-18:** CareNori, Access Care Navigator, Siden, Barry and CareBridge (bedside QR) all scored 27.5. Each has a strong idea or wide scope, but the writeups give less proof of depth or of what works.
- **Best unbuilt idea:** AccessCare telehealth (`todo-vbe71s`) compares two caption models and has a person settle disagreements. The author says most of it wasn't completed, so it placed 29th.

## Checks before announcing

The crawl doesn't include the event rules, so none of these affected the scores. Organizers should settle them before results go out.

| Project | Finding | What to do |
|---|---|---|
| SMS Shield | It is listed under four hackathons, and the writeup describes transforming it from "a simple medical billing and symptom-checking tool." | Check the repo history against the event window and the rules on prior work. If it is ineligible, everyone below moves up one and HealthBridge enters at 10th. |
| Accessible Medical Care Navigator and MediBridge | The same three people submitted both. | Check whether a team may enter twice. Only the Navigator placed in the top 10. |
| Accessible Medical Care Navigator | The crawl has a video but no repo or live link. | Watch the video to confirm its claims. |
| AcuPath | The hospital walkthrough is a disclosed simulation. | Confirm that the separate phone footage shows the working system. |
| CareBridge bedside QR (`carebridge-504tgi`) | The writeup describes hand-built HTML and JavaScript, but the tools listed are Base44 and Gemini. | No action needed unless it wins a prize. It placed 18th. |
| Medlexia | Its build section mentions "recipe management," apparently copied from another project. | Ask the team. It placed 24th. |
| Medicrate | It has no disability focus, and the writeup's React, Node and PostgreSQL stack conflicts with the listed Flask and Python. | No action needed. It placed 37th. |
| MedVoice | It claims real-time OCR but lists adding OCR models as future work. | No action needed. It placed 35th. |

Names also collide. There are three projects called CareBridge and two called AccessCare, so announcements should use the Devpost links.

## How stable the ranking is

**Doubling one criterion:** I reran the ranking four times, counting one criterion double each time. AcuPath stayed first every time. The same nine projects stayed in the top 10 every time. AccessAhead held tenth in three runs and lost it to HealthBridge when technical complexity doubled.

**Simulated panels:** I ran 50,000 simulated panels, each with random criterion weights and random judge disagreement on every score (standard deviation 0.75).

| Project | Median rank | Finished in top 10 |
|---|---|---|
| AcuPath | 1 | 98.5% |
| SMS Shield | 3 | 97.7% |
| Pawthfinder | 4 | 92.8% |
| HospitalRating | 5 | 92.7% |
| Clear Case | 6 | 86.5% |
| CareFit | 7 | 76.5% |
| HealthLens | 7 | 71.1% |
| Accessible Medical Care Navigator | 8 | 67.2% |
| Adaptive Touch | 8 | 64.7% |
| AccessAhead | 12 | 41.3% |
| HealthBridge | 13 | 30.9% |
| Cadence AI | 15 | 27.3% |
| AccessMed | 15 | 19.9% |

AcuPath finished first in 51.0% of panels, and SMS Shield was next at 19.4%. AccessAhead missed the top 10 more often than it made it, but it made it more often than any project ranked below it. This test only stresses my scores. It doesn't prove that a human panel would start from the same scores.

## Bias and limits

- **My own conflict:** I am a Claude model, and 7 of my top 10 mention Claude, compared with 10 of the other 40. I scored evidence and ignored the tool, but I can't rule out bias from my side. A human judge should look hard at HealthBridge and AccessMed, the highest-ranked projects outside the top 10 that don't mention Claude.
- **Writeup quality:** The crawl rewards teams that explained their work well. Beside, Barry, CareNav and Wayfind may be better than their writeups show.
- **Self-reported claims:** Test counts, accuracy figures and feature lists come from the teams, and I verified none of them. I only compared them for internal consistency.
- **No user evidence:** No team documents results from testing with disabled users. Every score here is a judgment about promise and evidence of the build, not proven benefit to patients.

## Appendix: all 50 scores

| Rank | Project | Devpost slug | P | C | S | T | Total | Note |
|---|---|---|---|---|---|---|---|---|
| 1 | AcuPath | `acupath` | 7.5 | 9.5 | 8.5 | 10 | 35.5 | Hardest build; solves physical navigation |
| 2 | SMS Shield | `sms-shield-gtks0o` | 8.5 | 8 | 9 | 8.5 | 34 | Most complete; eligibility check needed |
| 3 | Pawthfinder | `pawthfinder-qagtbu` | 7 | 9.5 | 8.5 | 8 | 33 | Most inventive portal tool; mock portal only |
| 4 | HospitalRating | `avaneesh-nelakosigi` | 8 | 9 | 8 | 7.5 | 32.5 | Generates missing data; needs real reviews |
| 5 | Clear Case | `carebridge-nih7wr` | 9 | 8 | 8 | 7 | 32 | Best document tool |
| 6 | CareFit | `carefit` | 7.5 | 7.5 | 8.5 | 7.5 | 31 | Best-built matcher; fictional clinics |
| 7 | HealthLens | `healthlens-q418rj` | 9 | 6.5 | 7.5 | 8 | 31 | Deployed and tested; common idea |
| 8 | Accessible Medical Care Navigator | `accessible-medical-care-navigator` | 8 | 7 | 7.5 | 8 | 30.5 | Measured OCR work; no repo in crawl |
| 9 | Adaptive Touch | `adaptive-touch` | 6.5 | 9 | 7 | 8 | 30.5 | Original tremor approach; limited reach |
| 10 | AccessAhead | `accessahead` | 7 | 8.5 | 8 | 5.5 | 29 | Strong concepts; build evidence is thin |
| 11 | HealthBridge | `healthbridge-sif8ny` | 7.5 | 6.5 | 7 | 7.5 | 28.5 | Real scanner and form helper |
| 12 | AccessMed | `accessmed` | 6.5 | 7 | 7.5 | 7 | 28 | Good extension; no real-portal evidence |
| 13 | Cadence AI | `cadence-ai-fa8n04` | 7 | 8.5 | 7.5 | 5 | 28 | Thoughtful aphasia design; no-code build |
| 14 | CareNori | `carenori` | 6.5 | 6.5 | 7 | 7.5 | 27.5 | Broad browser ML and maps; vague writeup |
| 15 | Access Care Navigator | `access-care-navigator` | 7 | 6.5 | 7.5 | 6.5 | 27.5 | Chat-to-booking flow; data source unstated |
| 16 | Siden | `maiden` | 7.5 | 6 | 7.5 | 6.5 | 27.5 | Useful voice health record; little technical detail |
| 17 | Barry | `barry-b5adrc` | 5.5 | 7.5 | 7.5 | 7 | 27.5 | Ambitious live advocate; thin proof |
| 18 | CareBridge (bedside QR) | `carebridge-504tgi` | 6.5 | 8.5 | 7 | 5.5 | 27.5 | Clever request routing; mock backend |
| 19 | Beside | `beside-tqjhzm` | 6.5 | 7 | 7 | 6 | 26.5 | Broad feature set by captions; near-empty writeup |
| 20 | Visage Health | `visage-health` | 6 | 7.5 | 7 | 6 | 26.5 | Face control for paralyzed patients; thin writeup |
| 21 | Medical Accessibility System | `what-should-we-make-our-team-name` | 6.5 | 7 | 7.5 | 5.5 | 26.5 | Local Gwinnett focus; dispatch is simulated |
| 22 | BenefitsBridge | `benefitsbridge-d5bzl2` | 6.5 | 7.5 | 7.5 | 5 | 26.5 | Life Simulator is fresh; limited depth |
| 23 | Careway | `medical-div` | 7.5 | 6 | 6.5 | 6 | 26 | Honest, private toolkit; no OCR or PDFs |
| 24 | Medlexia | `medilexa` | 7.5 | 5.5 | 6 | 6.5 | 25.5 | Solid dyslexia reader; copied writeup text |
| 25 | CareCost | `carecost-7j0q23` | 6 | 7 | 7 | 5.5 | 25.5 | Useful true-cost framing; data source unstated |
| 26 | What if? | `what-if-cgfxb1` | 5.5 | 8 | 6.5 | 5 | 25 | Inventive contingency planner; thin writeup |
| 27 | CareCompass | `carecompass-1donfj` | 7 | 5.5 | 6.5 | 5.5 | 24.5 | Broad generated site; voice issues noted |
| 28 | MediBridge | `medibridge-hv7tdq` | 7 | 4.5 | 6.5 | 6 | 24 | Working OCR, speech and captions; standard pieces |
| 29 | AccessCare (telehealth) | `todo-vbe71s` | 3.5 | 8.5 | 7 | 5 | 24 | Best unbuilt idea; mostly unfinished |
| 30 | VisitBridge | `visit-bridge` | 6.5 | 5.5 | 6 | 5.5 | 23.5 | Check-ins and scanning; limited depth |
| 31 | CareBridge Medical Assistant | `ringroom` | 6.5 | 5.5 | 6.5 | 4 | 22.5 | Real need; no staff side yet |
| 32 | AccessReady | `accesscare` | 5.5 | 4.5 | 6.5 | 5.5 | 22 | Facility matcher; focuses on styling |
| 33 | Cascade Navigation System | `tbd-mfpwt3` | 5 | 5.5 | 5.5 | 5 | 21 | Intake system; thin disability focus |
| 34 | Medical Care Voice Navigator | `medical-care-voice-navigator` | 5 | 5 | 5.5 | 4.5 | 20 | Voice Medicare help; small in scope |
| 35 | MedVoice | `medvoice-koway0` | 4.5 | 5 | 6 | 4 | 19.5 | Good concept; OCR unclear |
| 36 | CareBloom | `carebloom-2tvazc` | 4.5 | 5 | 4.5 | 5 | 19 | Gamified tasks; accessibility still to come |
| 37 | Medicrate | `medicrate` | 3 | 5 | 5 | 6 | 19 | Off-prompt; conflicting stack claims |
| 38 | Safe Space Stories | `safe-space-stories` | 3.5 | 7.5 | 6 | 1.5 | 18.5 | Good idea; no generator built |
| 39 | Prep Time | `prep-time-x3g1h9` | 4.5 | 5.5 | 5 | 3 | 18 | Simple rare-disease form |
| 40 | SimpleJargon | `simplejargon` | 4 | 4 | 4.5 | 4.5 | 17 | Post-visit portal; no disability focus |
| 41 | Diabetes Preventer for the Blind | `diabetes-preventer-for-the-blind` | 2.5 | 5 | 2.5 | 6.5 | 16.5 | Real classifier; three candies, off-prompt |
| 42 | VisitVoice | `visitvoice` | 4.5 | 3.5 | 5 | 2 | 15 | Basic speech buttons |
| 43 | CodeRidge_ADHD | `coderidge_adhd` | 3.5 | 3.5 | 3.5 | 3.5 | 14 | Journal from copied templates |
| 44 | Medical Jargon Translator | `medical-jargon-translator` | 3.5 | 2.5 | 4.5 | 3.5 | 14 | Q&A with no interface or accessibility features |
| 45 | CareNav | `carenav-2zymdw` | 3 | 2 | 3 | 2.5 | 10.5 | Writeup gives no specifics |
| 46 | Clinic Admitter | `clinic-admitter` | 2 | 2.5 | 3 | 2 | 9.5 | Small Java priority program |
| 47 | The Doctor Decoder | `the-doctor-decoder` | 2.5 | 1.5 | 2.5 | 1.5 | 8 | Static definitions of five medications |
| 48 | Memory Preservation Game | `memory-preservation-game` | 1 | 2 | 1.5 | 3 | 7.5 | Memory test; little information given |
| 49 | Care Helper | `care-helper` | 2 | 1.5 | 2 | 1.5 | 7 | Simple question-and-answer script |
| 50 | Wayfind | `wayfind-1nd92m` | 1 | 1 | 1 | 1 | 4 | Writeup is blank |
