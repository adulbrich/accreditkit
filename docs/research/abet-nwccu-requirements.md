# ABET and NWCCU: outcome text, evidence requirements, and pass rules

Research for [issue #2](https://github.com/adulbrich/accreditkit/issues/2). Investigated
2026-08-27 against primary sources only: ABET's own published criteria, self-study
questionnaire, and policy manual, and NWCCU's own standards, eligibility requirements,
policies, rubrics, and report guidelines. Every PDF and DOCX cited here was downloaded and
text-extracted locally rather than read through a summarizer, so the quoted text is verbatim.

Terms in **bold** are from [CONTEXT.md](../../CONTEXT.md).

## Bottom line

1. **ABET Student Outcomes for a CS Systems program are outcomes 1 through 5 of the general
   computing criteria plus Computer Science outcome 6, and nothing else.** Cycle is
   2026-2027. Program Criteria key on the *program title*, and there is no Systems entry in
   the Computing Accreditation Commission's Program Criteria, so a Systems concentration
   below a Computer Science degree title adds no outcomes. Verbatim text in section 1.

2. **ABET mandates a documented assessment and evaluation process and a stated expected level
   of attainment per Student Outcome. It does not mandate the Performance Indicator
   construct and does not set any threshold.** The words "performance indicator",
   "threshold", "benchmark", and "target" appear zero times in both the 2026-2027 CAC
   Criteria and the 2026-2027 CAC Self-Study Questionnaire. **This corrects CONTEXT.md,
   which says Performance Indicators are "Required by ABET".** ABET's pass rule is a peer
   evaluator's per-criterion finding of Deficiency, Weakness, Concern, or Observation, not a
   computation over data.

3. **NWCCU specifies no pass / not-pass rule for outcome achievement. Not specified by
   NWCCU.** No threshold, percentage, count of measures, or per-outcome decision procedure
   exists in the 2020 Standards, the 2020 Eligibility Requirements, the Accreditation
   Criteria Policy, the Handbook of Accreditation, the EIE (Year Seven) Guidelines, the
   Mid-Cycle Guidelines, or any of NWCCU's three published rubrics (1.B.1 to 1.B.4, 1.C.1 to
   1.C.9, 1.D.1 to 1.D.4). The rubrics that exist rate the maturity of the *institution's
   assessment system* on a four level scale, not the attainment of any one outcome. **I found no primary source for the
   "two Data Points per Student Outcome" claim anywhere in NWCCU's published corpus.**

4. **Whether an NWCCU Data Point must be a direct measure is not specified by NWCCU.** The
   word "indirect" appears zero times in the 2020 Standards, the 1.C rubric, the EIE
   Guidelines, and the Mid-Cycle Guidelines. NWCCU's "Direct Assessment and
   Competency-Based Education" policy is a false friend: it governs Title IV credit-hour
   equivalence for CBE programs, not direct versus indirect measurement of learning. ABET,
   by contrast, explicitly permits both. Practitioner knowledge has since resolved this the
   other way inside CONTEXT.md; see section 6.

5. **NWCCU accredits the institution, not the program, and program-level reporting reaches
   NWCCU only as evidence inside institution-level standards.** Handbook of Accreditation:
   "Institutional accreditation applies to an institution as a whole, not individual
   programs or units within the institution." Standard 1.C.5 obliges the institution to
   assess "the quality of learning in its programs", and the Mid-Cycle Report requires a
   sample of "at least two programs". Notably, that same guideline says programs approved by
   a CHEA-recognized programmatic accreditor "are not needed for this report", which
   excludes an ABET-accredited CS program from the sample.

---

## 1. ABET Student Outcomes for a Computer Science program with a Systems concentration

**Source:** ABET, *Criteria for Accrediting Computing Programs, Effective for Reviews during
the 2026-2027 Accreditation Cycle*, "Incorporates all changes approved by the ABET Board of
Delegates Computing Area Delegation as of October 24, 2025", copyright 2025.
Landing page: <https://www.abet.org/accreditation/accreditation-criteria/criteria-for-accrediting-computing-programs-2026-2027/>
PDF: <https://www.abet.org/wp-content/uploads/2025/12/2026-2027_CAC_Criteria.pdf>

### Criterion 3. Student Outcomes (General Criteria, baccalaureate level), verbatim

> The program must have documented and publicly stated student outcomes that include (1)
> through (5) below and any outcomes required by applicable Program Criteria. The program may
> define additional outcomes.
>
> Graduates of the program will have an ability to:
>
> 1. Analyze a complex computing problem and apply principles of computing and other
>    relevant disciplines to identify solutions.
> 2. Design, implement, and evaluate a computing-based solution to meet a given set of
>    computing requirements in the context of the program's discipline.
> 3. Communicate effectively in a variety of professional contexts.
> 4. Recognize professional responsibilities and make informed judgments in computing
>    practice based on legal and ethical principles.
> 5. Function effectively as a member or leader of a team engaged in activities appropriate
>    to the program's discipline.

### Computer Science Program Criteria, verbatim

Section IV, "Computer Science and Similarly Named Computing Programs", Lead Society: CSAB:

> These program criteria apply to computing programs using computer science or similar terms
> in their titles.
>
> **3. Student Outcomes**
>
> In addition to outcomes 1 through 5, graduates of the program will also have an ability to:
>
> 6. Apply computer science theory and software development fundamentals to produce
>    computing-based solutions. [CS]

### Does a Systems concentration add outcomes? No.

Program Criteria attach to the program title, not to a concentration. Section IV opens:

> All programs seeking accreditation from the Computing Accreditation Commission of ABET must
> demonstrate that they satisfy all of the specific Program Criteria implied by the program
> title.

The document's Program Criteria are exactly: Computer Science, Cybersecurity (associate),
Cybersecurity, Data Science / Data Analytics, Information Systems, Information Technology
(associate), and Information Technology. **There is no Systems program criteria section.** A
Systems concentration under a Computer Science degree title therefore contributes no
additional Student Outcome. The full set for CS Systems is outcomes 1 through 6.

Two caveats worth recording in the app's data model:

- The program *may* define additional outcomes ("The program may define additional
  outcomes"). Any Systems-specific outcome a program carries is Program-authored, not
  Accreditor-authored. That collides with CONTEXT.md's rule that a **Student Outcome** is
  "never authored inside the app", and needs a decision.
- Section V of the same PDF carries *Proposed Changes to the Criteria* not yet in effect,
  including proposed program criteria for Artificial Intelligence / Machine Learning and a
  proposed revision to Information Systems. ABET's own note says the adopted criteria become
  effective after the fall 2026 Computing Area Delegation meeting and are first applied in
  the 2027-28 review cycle. 2026-2027 is confirmed as the most recent published computing
  cycle; no 2027-2028 criteria exist yet
  (<https://www.abet.org/accreditation/accreditation-criteria/>). The same document also
  carries separate outcome sets for other degree levels at Criterion MS3 (master's) and
  Criterion MI3. Verbatim outcome text is therefore keyed by accreditor plus cycle year plus
  degree level, and the app must store all three alongside the text. CONTEXT.md's **Program**
  definition currently mentions none of them.

## 2. What ABET requires as evidence that a Student Outcome is met

### The mandate lives in Criterion 4, and it is thin

*2026-2027 CAC Criteria*, Criterion 4. Continuous Improvement, verbatim:

> The program must regularly use appropriate, documented processes for assessing and
> evaluating the extent to which the student outcomes are being attained. The results of
> these evaluations must be systematically utilized as input for the program's continuous
> improvement actions. Other available information may also be used to assist in the
> continuous improvement of the program.

The same document's Definitions section, verbatim:

> **Assessment**
> Assessment is one or more processes that identify, collect, and prepare data to evaluate
> the attainment of student outcomes. Effective assessment uses relevant direct, indirect,
> quantitative and qualitative measures as appropriate to the outcome being measured.
> Appropriate sampling methods may be used as part of an assessment process.
>
> **Evaluation**
> Evaluation is one or more processes for interpreting the data and evidence accumulated
> through assessment processes. Evaluation determines the extent to which student outcomes
> are being attained. Evaluation results in decisions and actions regarding program
> improvement.

That is the whole mandate. It requires a process, requires it to be documented, requires it
to be regular, and requires the results to feed improvement. It names no unit of measurement.

### What the self-study expects

**Source:** ABET, *Self-Study Questionnaire: Template for a Self-Study Report, Computing
Accreditation Commission, 2026-2027* (document C002B, dated 2025-12).
<https://www.abet.org/wp-content/uploads/2026/01/C002B_CAC-Self-Study-Questionnaire_2026-2027_2025-12.docx>

Criterion 3 in the questionnaire asks only for two things: list the Student Outcomes
including any the program defined beyond the required set, and describe where they are
publicly stated.

Criterion 4 is where the evidence expectation sits. Verbatim, including the hedge:

> Although the program can report its processes as it chooses, the following is presented as
> a guide to help you organize your Self-Study Report.
>
> **Student Outcomes**
>
> It is recommended that this section include (a table may be used to present this
> information):
>
> - A listing and description of the assessment processes used to gather the data upon which
>   the evaluation of each student outcome is based for the students within the program and
>   disaggregated by the students in the program under review. Examples of data collection
>   processes may include, but are not limited to, specific exam questions, student
>   portfolios, internally developed assessment exams, senior project presentations,
>   nationally-normed exams, oral exams, focus groups, industrial advisory committee
>   meetings, or other processes that are relevant and appropriate to the program.
> - The frequency with which these assessment processes are carried out
> - The expected level of attainment for each of the student outcomes
> - Summaries of the results of the evaluation process and an analysis illustrating the
>   extent to which each of the student outcomes is being attained
> - How the results of the assessment process are documented and maintained
> - How and where the student outcome assessment process is documented

And on availability of the underlying artifacts:

> Copies of any of the assessment instruments or materials referenced in 4.A. and 4.B must be
> available for review at the time of the visit.

The questionnaire is an aid, not itself a requirement. *2026-2027 APPM* section I.D.1.f:
"To assist programs in completing a Self-Study Report, each commission has developed a
Self-Study Questionnaire that is posted on the ABET website."
(<https://www.abet.org/wp-content/uploads/2025/11/2026-2027_APPM.pdf>)

### Performance Indicators and thresholds: not mandated by ABET

I grepped both documents. Results:

| term | 2026-2027 CAC Criteria | 2026-2027 CAC SSQ |
| --- | --- | --- |
| "performance indicator" | 0 | 0 |
| "indicator" | 0 | 0 |
| "threshold" | 0 | 0 |
| "benchmark" | 0 | 0 |
| "target" | 0 | 0 |
| "rubric" | 0 | 1 (Criterion 5 display materials list) |
| "expected level of attainment" | 0 | 1 |

The only quantity-shaped requirement anywhere in ABET's evidence expectation is "The
expected level of attainment for each of the student outcomes", and it appears in the
*recommended* section of a *questionnaire*, with no value attached. **ABET mandates no
threshold. The program sets its own expected level of attainment and ABET evaluates whether
the program's own process is sound and documented.**

Decomposing a Student Outcome into **Performance Indicators** is widespread practice among
computing programs and is what most ABET assessment consultants teach, but it is not an ABET
requirement. Treat it as common practice, not mandate.

### ABET's pass rule is a human finding, not a computation

*2026-2027 APPM*, section I.E.8.a, verbatim:

> **I.E.8.a.(2)(a) Deficiency** – A Deficiency indicates that a criterion, policy, or
> procedure is not satisfied. Therefore, the program is not in compliance with the criterion,
> policy, or procedure.
>
> **I.E.8.a.(2)(b) Weakness** – A Weakness indicates that a program lacks the strength of
> compliance with a criterion, policy, or procedure to ensure that the quality of the program
> will not be compromised. Therefore, remedial action is required to strengthen compliance
> with the criterion, policy, or procedure prior to the next review.
>
> **I.E.8.a.(2)(c) Concern** – A Concern indicates that a program currently satisfies a
> criterion, policy, or procedure; however, the potential exists for the situation to change
> such that the criterion, policy, or procedure may not be satisfied.
>
> **I.E.8.a.(3) Findings of Observation** – An Observation is a comment or suggestion that
> does not relate directly to the current accreditation action but is offered to assist the
> institution in its continuing efforts to improve its programs.

Note the unit: findings attach to a *criterion*, not to a Student Outcome. A program does not
"pass Outcome 3". A program either satisfies Criterion 4 or does not, and a peer evaluator
decides. **This matters for the accreditor seam.** The ticket frames the seam as abstracting
over two different pass rules. ABET's is not a rule over data at all. What ABET actually
constrains is the *shape of the self-study*: process description, frequency, stated expected
level of attainment, results summary, and retrievable instruments.

The "threshold" that CS programs typically state, such as "70 percent of sampled students at
or above Proficient", is the program's own answer to "expected level of attainment". It is
Program-authored data, and the app should model it as such rather than as an Accreditor
constant.

## 3. NWCCU's pass / not-pass rule for outcome achievement

**Finding: not specified by NWCCU.** NWCCU publishes no per-outcome pass rule, no threshold,
and no required number of measures.

I searched the following primary sources and found no threshold, percentage, minimum count of
measures, or per-outcome decision procedure in any of them:

- *NWCCU 2020 Standards for Accreditation*, Standards 1.A through 2.I.
  <https://nwccu.org/standards/>
- *NWCCU 2020 Eligibility Requirements*, all 23.
  <https://nwccu.org/accreditation/standards-policies/eligibility-requirements/>
- *Accreditation Criteria Policy*, revised May 2025.
  <https://nwccu.box.com/s/6q8m37amhe66bjlnisvom9m8axz29ymy>
- *The Handbook of Accreditation*, updated January 22, 2026.
  <https://nwccu.box.com/s/lcp7r49i8409za7bt0jeqx0zbpf89eyi>
- *Guidelines: Preparing Evaluation of Institutional Effectiveness (EIE) Reports*, revised
  June 2023. <https://nwccu.box.com/s/1x331sxkvw1s64leo0ew571kgwe12zpt>
- *Guidelines: Preparing Mid-Cycle Reports*, revised June 2023.
  <https://nwccu.box.com/s/wc8wojotbw7pwt19xx3vnhnohlujys5x>
- *Rubric for Standards 1.B.1 to 1.B.4*.
  <https://nwccu.box.com/s/wb5ox9h7bet2yghsqqw8q35xyotpfm0u>
- *Rubric for Student Learning, Standards 1.C.1 to 1.C.9*.
  <https://nwccu.box.com/s/gbj5waxtyignubvkjqi9ufq3cknadxgr>
- *Rubric for Standards 1.D.1 to 1.D.4*.
  <https://nwccu.box.com/s/sfj5v8nlkp5199sx9hzz6z23ip33dfy8>
- The full NWCCU policy index. <https://nwccu.org/policies/>

### What NWCCU actually requires

The relevant standards, verbatim from <https://nwccu.org/standards/>:

> **1.C.5** The institution engages in an effective system of assessment to evaluate the
> quality of learning in its programs. The institution recognizes the central role of faculty
> to establish curricula, assess student learning, and improve instructional programs.

> **1.C.7** The institution uses the results of its assessment efforts to inform academic and
> learning-support planning and practices to continuously improve student learning outcomes.

> **1.B.1** The institution demonstrates a continuous process to assess institutional
> effectiveness, including student learning and achievement and support services. The
> institution uses an ongoing and systematic evaluation and planning process to inform and
> refine its effectiveness, assign resources, and improve student learning and achievement.

And Eligibility Requirement 5, verbatim from
<https://nwccu.org/accreditation/standards-policies/eligibility-requirements/>:

> **STUDENT LEARNING:** The institution identifies and publishes the expected learning
> outcomes for each of its degree, certificate, or credential programs. The institution
> engages in regular and ongoing assessment to validate student learning and, consistent with
> its mission, the institution establishes and assesses student learning outcomes (or core
> competencies) examples of which include, but are not limited to, effective communication,
> global awareness, cultural sensitivity, scientific and quantitative reasoning, critical
> analysis and logical thinking, problem solving, and/or information literacy that are
> assessed across all associate and bachelor level programs or within a General Education
> curriculum.

Every operative phrase is a system property: "an effective system of assessment", "a
continuous process", "regular and ongoing assessment". None of them is a per-outcome verdict.

### The closest thing NWCCU has to a rule is a maturity rubric, and it rates the system

NWCCU publishes a *Rubric for Student Learning, Standards 1.C.1 to 1.C.9* with four columns:
Initial, Emerging, Developed, Highly Developed. The 1.C.5 row, verbatim:

> **1.C.5 An effective system of assessment of the quality of learning.**
>
> - *Initial:* Assessment of learning is done at the course level with little or no
>   interaction across departments to discuss learning overall.
> - *Emerging:* Academic departments and programs assess student learning within the courses
>   and sequences of courses under their purview. Some cross-disciplinary discussion of
>   student learning occurs, particularly when courses are prerequisites or program
>   requirements.
> - *Developed:* The institution monitors assessment plans and reports and documents the use
>   of results to improve learning outcomes across academic departments; common assessment
>   elements such as rubrics exist.
> - *Highly Developed:* The institution has a well-defined system for evaluating the
>   effectiveness of its learning assessment plans, including training, timelines for review,
>   scoring rubrics, and accountability measures across academic departments.

The rubric's stated purpose is "to support institutions and peer review teams in assuring
student learning". It contains no percentage, no count of measures, and no direct versus
indirect distinction. The companion rubrics for 1.B and 1.D are the same shape and contain
neither "threshold" nor "indirect"; the single "at least" in the 1.D rubric is about
coordination between student service units and is unrelated to measurement.

**Consequence for the accreditor seam:** there is no NWCCU pass function to implement. What
NWCCU wants demonstrated is that the Program has a **Determination** process that runs, that
it is documented, and that its results changed something. The seam should not assume both
accreditors expose a `passes(outcome, data) -> bool`. NWCCU's side is closer to
`describesProcess()` plus `showsUseOfResults()`.

### The "two Data Points per Student Outcome" claim

**Not found in any NWCCU primary source.** I searched the standards, ERs, handbook, criteria
policy, both report guidelines, and the 1.C rubric. There is no "two", no "at least two
measures", and no "data point" language attached to outcomes anywhere.

The nearest published NWCCU rule that uses the number two is in the *Mid-Cycle Guidelines*
and it counts **programs, not measures**:

> The institution describes its assessment framework and must provide programmatic assessment
> of at least two programs as evidence of a continuous process of improvement.

That is one plausible origin for a misremembered "two data points". I am flagging it as a
hypothesis, not a finding. Record the assessment faculty's answer as practitioner knowledge
when it arrives, and label it as institutional practice or as a specific NWCCU staff liaison's
guidance, not as a published NWCCU requirement, because it is not one.

### Reconciliation with the Assessment Faculty's parallel answer

The Assessment Faculty answered items 3 and 4 in
[issue #2](https://github.com/adulbrich/accreditkit/issues/2#issuecomment-5440492731) while
this investigation ran. Their item 3 answer, hedged with "I think", was **"Over 70% of
students score over 70%"**. The primary sources settle it:

- **The 70/70 rule is not NWCCU's.** No threshold of any value appears anywhere in NWCCU's
  published corpus. NWCCU does not mandate this rule, a different rule, or any rule.
- **Therefore it is the Program's own rule**, and it is exactly the same kind of object as
  the "expected level of attainment" ABET asks a program to state. It is Program-authored
  configuration that **Assessment Faculty** must be able to edit, not **Accreditor** content,
  and it does not belong in the accreditor seam.
- **Both accreditors accept the same rule form.** "X percent of students at or above level Y"
  satisfies ABET's "expected level of attainment" and is unobjectionable to NWCCU, which asks
  only that the process exist, be documented, and drive change. The seam does not need to
  abstract over two different threshold computations, because only one side has one and the
  Program owns it.

That collapses most of the difficulty the ticket anticipated. The real asymmetry between the
two accreditors is not the pass arithmetic. It is *what gets reported*: ABET wants a
per-criterion self-study with retrievable instruments, and NWCCU wants a program report the
institution can cite as evidence under Standard 1.C.5.

## 4. Must an NWCCU Data Point be a direct measure?

**Finding: not specified by NWCCU.**

The word "indirect" appears **zero times** in the 2020 Standards, the Rubric for Standards
1.C.1 to 1.C.9, the EIE Guidelines, and the Mid-Cycle Guidelines. NWCCU never draws the
direct-versus-indirect distinction in its normative documents, so it neither requires direct
measures nor blesses indirect ones.

**Do not misread the CBE policy.** NWCCU's *Direct Assessment and Competency-Based Education
Policy* (revised March 2023, <https://nwccu.box.com/s/cjnwj3ms3c9hu7sv3iy007jkbov473dc>) uses
"direct assessment" in the federal Title IV sense, quoting what it renders as 34 CFR 688.10(a):

> Direct assessment of student learning means a measure of a student's knowledge, skills, and
> abilities designed to provide evidence of the student's proficiency in the relevant subject
> area.

but its subject is credit-hour equivalence for competency-based programs, not the direct
versus indirect measurement taxonomy used in outcomes assessment. Citing it as evidence that
NWCCU requires direct measures would be wrong.

### NWCCU-published guidance, non-normative

NWCCU's newsletter article *Demystifying NWCCU's Assessment Standards*
(<https://nwccu.org/news/v5i4-demystifying-nwccus-assessment-standards/>) describes
institutions in early stages as "typically using more indirect measures of assessment, and
few if any direct measures", listing that among characteristics of less mature programs. This
implies a preference for direct measures. It is first-party but it is a newsletter, not a
standard, and it does not create a requirement. **Label: NWCCU-published guidance,
non-normative.**

### ABET, by contrast, explicitly permits indirect

From the CAC Criteria Definitions quoted in section 2: "Effective assessment uses relevant
direct, indirect, quantitative and qualitative measures as appropriate to the outcome being
measured." The SSQ's list of example data collection processes explicitly includes "focus
groups" and "industrial advisory committee meetings", both indirect.

### Architectural consequence, as inference

This is my inference from the findings above, not an accreditor requirement:

If NWCCU does not require direct measures and ABET explicitly permits indirect ones, then a
**Data Point** can legitimately come from an alumni survey or an exit interview, and such a
Data Point has no **Course Offering** behind it. That collides directly with CONTEXT.md's
rule that "Evidence is always attached to an Offering". The collision is real regardless of
how NWCCU is read, because ABET's definition of Assessment settles it for the ABET side.

## 5. NWCCU program-level reporting versus institution-level review

### The mechanism

NWCCU accredits the institution. *The Handbook of Accreditation* (updated January 22, 2026),
page 11, verbatim:

> Institutional accreditation applies to an institution as a whole, not individual programs or
> units within the institution.

Page 12 draws the contrast with ABET explicitly:

> Specialized or programmatic accrediting agencies accredit individual educational programs
> within an institution with regard to program-specific standards (e.g., business, law,
> engineering, nursing).

There is no NWCCU program accreditation, no program self-study submitted to NWCCU, and **no
program review policy in NWCCU's published policy index** (I enumerated all 38 policies at
<https://nwccu.org/policies/>; program review is absent).

Program-level reporting exists because institution-level standards are *satisfied by
program-level evidence*. Standard 1.C.5 requires the institution to assess "the quality of
learning in **its programs**", and 1.C.3 requires it to publish "expected program and degree
learning outcomes for all degrees, certificates, and credentials". A program's assessment
report is therefore an internal institutional artifact that the institution aggregates and
cites. The program reports to the institution; the institution reports to NWCCU.

### Where program evidence actually surfaces to NWCCU

Three named touchpoints, all institution-level submissions:

1. **Mid-Cycle Report** (*Guidelines: Preparing Mid-Cycle Reports*, revised June 2023),
   component 5, "Programmatic Assessment", verbatim:

   > The institution describes its assessment framework and must provide programmatic
   > assessment of at least two programs as evidence of a continuous process of improvement.
   > The programs should be broadly representative of institutional efforts. Note that
   > programs approved by a CHEA-recognized programmatic accreditor are not needed for this
   > report.

   **The last sentence is load-bearing for this project.** ABET is CHEA-recognized, so an
   ABET-accredited CS program is explicitly excluded from the Mid-Cycle sample. NWCCU defers
   to the programmatic accreditor here rather than duplicating it.

2. **EIE / Year Seven Report** (*Guidelines: Preparing Evaluation of Institutional
   Effectiveness (EIE) Reports*, revised June 2023), component 5.c, Standard 1.C, sub-item
   iii, verbatim:

   > Evidence of an effective system of assessment of student learning in programs with
   > faculty establishing curricula, assessing student learning, and improving instructional
   > programs.

   The EIE is "a comprehensive, summative evaluation of the institution, occurring in the
   seventh year of the accreditation cycle" and is typically 30 to 45 pages for the entire
   institution. That page budget is itself evidence that no single program's outcome data
   reaches NWCCU in detail; what reaches NWCCU is the framework plus exemplars.

3. **Substantive Change** (*Substantive Change Policy*, revised August 2025,
   <https://nwccu.box.com/s/9j3snl0v7hvk8g3e2t6k3ywmv1nk24fb>) is the mechanism by which a
   specific new or materially changed degree program comes before NWCCU as a program. It is
   an approval gate, not an assessment report.

### Consequence for the app

A Program's NWCCU-facing output is not a submission to NWCCU. It is an artifact the
institution's accreditation liaison officer can pull into a Mid-Cycle or EIE report, or file
as an exhibit. So the NWCCU **Accreditor** configuration should be understood as "produce a
program assessment report in a form the institution can cite", with the reporting **Assessment
Cycle** cadence set by the institution, not by NWCCU.

## 6. Corrections and collisions with CONTEXT.md

Three, in order of how much they move architecture.

1. **"Performance Indicator ... Required by ABET" is wrong.** ABET requires a documented
   assessment and evaluation process and, in a recommended self-study section, a stated
   expected level of attainment per Student Outcome. It never names Performance Indicators.
   Both accreditors leave the construct optional. Keeping Performance Indicators in the model
   is defensible on practice grounds, but the justification is "this is how programs actually
   organize evidence and how ABET evaluators expect to read it", not "ABET requires it".

2. **"Data Point ... NWCCU requires at least two per Student Outcome" has no primary source.**
   Section 3. Carry it as practitioner knowledge if the assessment faculty confirm it.

3. **CONTEXT.md changed during this investigation** to define a **Data Point** as "One direct
   measurement supporting a Student Outcome, produced by a Course Offering ... Indirect
   measures such as surveys and exit interviews do not count." That is a valid project
   decision and I am not contradicting it, but it should be recorded as *practitioner
   knowledge or project policy*, not as an accreditor requirement, because:
   - NWCCU does not specify direct versus indirect at all (section 4).
   - ABET's Definitions section explicitly permits indirect measures, so an ABET self-study
     can and often does cite exit interviews and employer surveys. If the app cannot hold
     them as Data Points, they live outside the app and the ABET report is assembled from two
     places.

   Recommend surfacing that trade-off to the assessment faculty before it hardens.

## Appendix: retrieval notes

- ABET criteria, SSQ, and APPM were downloaded and extracted with `pdftotext -layout` and, for
  the DOCX, by unzipping `word/document.xml`. Quotes are from those extractions.
- NWCCU documents hosted on Box are reachable directly at
  `https://nwccu.box.com/shared/static/<share-id>.pdf`, using the share id from the
  `nwccu.box.com/s/<id>` link on the NWCCU page.
- The only non-normative source used is the NWCCU newsletter article in section 4, and it is
  labeled as such. No university summaries, blogs, or slide decks were used.
