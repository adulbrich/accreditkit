# accreditkit

Helps university faculty run program accreditation assessment: collect evidence from the
faculty who teach courses, judge it with a reasoning model as an advisor, and let the
faculty who report to accreditors make and record the actual determination.

Terms below are settled. Anything not listed here is still open; see the
[wayfinder map](https://github.com/adulbrich/accreditkit/labels/wayfinder%3Amap).
Accreditor facts here are sourced from
[docs/research/abet-nwccu-requirements.md](./docs/research/abet-nwccu-requirements.md).

## Language

### Program and accreditation

**Program**:
The top-level scope that owns everything else: a degree program under assessment, such as
CS Systems. One deployment serves one institution and many Programs.
_Avoid_: Department, tenant, organization

**Accreditor**:
A body a Program reports to, such as ABET or NWCCU. Accreditors differ in what they require
reported and at what scope, and may share a Student Outcome set. Neither ABET nor NWCCU
computes pass from data: ABET pass is a peer evaluator's per-criterion finding, and NWCCU
accredits the institution rather than the Program. Any numeric threshold in this system is the
Program's own.
_Avoid_: Standard, accreditation body, agency

**Student Outcome**:
A statement of what students are expected to be able to do by graduation, numbered and
quoted verbatim from the Accreditor. Shared across Accreditors where they agree, and
never authored inside the app.
_Avoid_: Learning outcome, program outcome, ABET outcome, competency

**Performance Indicator**:
A measurable, Program-authored statement of what evidence demonstrates a Student Outcome.
Authored once at the Program level and reused across Assessment Cycles. Neither ABET nor
NWCCU mandates the construct; it is how programs in practice organize evidence and how ABET
evaluators expect to read it.
_Avoid_: PI (in prose), criterion, measure, benchmark

### Courses

**Course**:
A catalog entry, such as CS 344. Stable across terms and independent of who teaches it.
_Avoid_: Class, subject

**Course Offering**:
One delivery of a Course in one term by one instructor, such as CS 344 Fall 2026. Evidence
is always attached to an Offering, never to a Course.
_Avoid_: Section, class, instance, run

**Course Learning Outcome**:
A statement of what students are expected to be able to do by the end of a specific
Course. Authored by faculty, distinct from a Student Outcome, and mapped upward to
Performance Indicators or Student Outcomes.
_Avoid_: CLO (in prose), objective, course goal

**Curriculum Map**:
The Program's standing declaration of which Courses count toward accreditation and how
their Course Learning Outcomes map upward. Changes rarely; an Assessment Cycle records
the version it ran against.
_Avoid_: Coverage matrix, alignment map, crosswalk

### Assessment

**Assessment Cycle**:
The bounded period, generally one year, over which evidence is collected and a Program
reaches its determinations. Reports to an Accreditor are made per Cycle.
_Avoid_: Period, review, assessment year, cohort

**Evidence Artifact**:
Something produced by a Course Offering that can support a Course Learning Outcome, such
as an assignment, its rubric, or a syllabus.
_Avoid_: Document, submission, material

**Rubric Criterion**:
One row of a rubric on an Evidence Artifact. The finest granularity at which evidence is
mapped and measured.
_Avoid_: Rubric item, rubric line, criteria (as singular)

**Data Point**:
One direct measurement supporting a Student Outcome, produced by a Course Offering. May be as
fine-grained as a single Rubric Criterion. Indirect measures such as surveys and exit
interviews do not count, and at least two are expected per Student Outcome. Both of those are
this project's policy, not accreditor requirements: NWCCU specifies neither, and ABET
explicitly permits indirect measures.
_Avoid_: Measure, sample, metric

**Achievement Data**:
How students actually performed against a Rubric Criterion, collected separately from and
later than the Evidence Artifact itself.
_Avoid_: Grades, scores, results, performance data

**Assessment Run**:
One execution of the reasoning model over a Course Offering's Evidence Artifacts, producing
advisory findings. Immutable once complete, and never authoritative on its own.
_Avoid_: Evaluation, analysis, AI review, scan

**Determination**:
A human judgment of record, made by Assessment Faculty and always attributable. May
reference an Assessment Run and may contradict it. Made at two levels: on a single Course
Offering's submission, and on a Student Outcome across an Assessment Cycle.
_Avoid_: Verdict, decision, score, go/no-go, sign-off

### People

**Assessment Faculty**:
The Program-level role that authors Performance Indicators and the Curriculum Map,
configures Accreditors, opens and closes Assessment Cycles, makes Determinations, and
reports to Accreditors. Every record in the system is editable by this role.
_Avoid_: Judge, reviewer, coordinator, admin

**Instructor**:
A relationship, not a role: the person of record for a specific Course Offering, which is
what grants the right to submit its evidence. Assessment Faculty are routinely also
Instructors.
_Avoid_: Teacher, faculty (unqualified), owner
