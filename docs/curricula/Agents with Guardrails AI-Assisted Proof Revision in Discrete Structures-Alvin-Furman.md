# Agents with Guardrails: AI-Assisted Proof Revision in Discrete Structures

## Furman University
Contributed by Chris Alvin (chris.alvin@furman.edu), Mark Johnson (mark@fellowhumans.com), Tram Le (letr9@furman.edu), and Andrew O'Dell (odean8@furman.edu)

## Institutional and departmental context
- Location: Greenville, South Carolina, USA
- Undergraduate student body size: 2,500 students
- Degree(s) offered: B.A. and B.S. in Computer Science; B.A. and B.S. in Information Technology; B.S. in Artificial Intelligence; B.S. in Data Science
- Department/major name: Department of Computer Science
- Number of contributing faculty: 1.5 FTE (course instructor and adjunct)
- Number of majors annually: 30 to 35 across the department
- Does the department offer any graduate programs? No
- Other context: Furman launched a B.S. in Artificial Intelligence in Fall 2026, and Discrete Structures is required for CS and the new AI major. Johnson developed PathMX, a curriculum-as-code platform [1], which the department uses in CS0, CS1, and an upper-level AI course, and now Discrete Structures. A companion SIGCSE TS 2027 paper [2] places three PathMX deployments on a continuum from instructor-defined structure to student-defined work. Discrete Structures sits at the structured end and tests whether guardrails preserve understanding. Campus AI guidance sets permitted AI use at the assignment level, which lets this course require agent use on homework while prohibiting it on exams.

## Description of Curricular Innovation

**The problem.** In proof-based courses, generative AI can produce a correct final proof without the student performing the reasoning. Grading homework for correctness therefore measures less than it once did. Discrete Structures (CSC-261) is often the first course in which our students must write proofs, so the habits they form here carry into later theory courses. In a related deployment in an upper-level course, some students reported that relying on an agent reduced their understanding of their own code, while others learned to question the agent [2]. A proof course needs a design that produces the second outcome.

**The workflow.** Students write each solution by hand first, photograph it, and upload the image to PathMX, which converts it to LaTeX. The handwritten draft is deliberate. Writing by hand mirrors how students already work, and the photograph-and-upload step slows students down so that their own reasoning exists before any agent sees the problem. Students then refine that LaTeX with an AI coding agent (OpenAI Codex). The workflow applies to all homework problems, including coding problems.

**The guardrails.** The agent works only on a student's own handwritten attempt; it does not originate the solution. It returns feedback on the structure and validity of a drafted proof and helps with LaTeX mechanics. The student decides what to revise. A course objective makes this explicit: students assess the feedback critically rather than adopting it without verification. The agent is the only generative AI tool permitted on graded work, and no AI tool is permitted on exams. Students may not ask any tool to solve a problem similar to an open homework problem, and they cite their use of the agent on each submission. Each submission carries a verification and honesty checklist in which students attest to what they checked themselves and whether they took any shortcuts.

Students are responsible for the following verification checks:

- Compare the automatic LaTeX transcription with their own handwritten attempt and correct any errors.
- Decide how to act on the agent's suggestion, explaining the choice in their own words.
- Check every statement in their final proof.
- Ensure they can explain the key inference without referring back to the agent's conversation.
- Review the agent's summary of the revision process and correct inaccuracies before approving it.

**Assessment redesign.** Homework is graded for correctness but carries only 15% of the course grade. Proctored exams, on which no AI tool is permitted, carry 75%: three midterm exams at 45% and a final exam at 30%. Professionalism is 10%. To pass, a student must earn at least half of the available points in each component, so strong homework cannot offset weak exam performance. Homework problems are unchanged from prior offerings; only the workflow changed. This assessment structure does not depend on PathMX and can be adopted in any problem-based course.

**Liberal arts framing.** The course enrolls 19 students, which allows close attention to each student's reasoning. The design treats AI as a tool that students must direct and own, rather than a tool to prohibit. Judging a source critically and defending an argument in one's own words are liberal arts habits, and the workflow makes both a routine part of proof writing. The course uses no AI detection software. When a submission does not resemble a student's other work, the first step is a conversation in which the student walks through the argument; if the student can explain it, the matter ends there.

**Evaluation in progress.** Alvin and Johnson lead the study with two undergraduate research assistants, Le and O'Dell, who co-designed the surveys and data plan and are not enrolled in the course. We ask three research questions: whether students retain understanding (RQ1), whether skills transfer beyond the AI-assisted workflow (RQ2), and whether students maintain integrity and responsibility for their reasoning (RQ3). Students complete an 8-item pre-survey and a 10-item post-survey on proof self-efficacy, reliance, transfer, and verification. Study codes link surveys, homework logs, and exam scores; participation does not affect grades, and analysis begins after final grades are submitted. Prior offerings provide an informal baseline: Alvin observes that homework this semester is stronger overall. Agent-assisted revision could produce that difference without any gain in understanding; proctored exam performance will show whether students retain the reasoning on their own. Exam 1 offers an early caution. Students performed poorly on proof by cases and were weak on proof by contradiction and contraposition. Many also struggled with the algebra in induction proofs.

## Challenges/Limitations

**Challenges we face.**

- The study involves a single section of 19 students (20 at the start of the term), which limits generalization.
- The verification and honesty checklist relies on student self-report.
- Study results are not available until after the semester ends.
- Protecting student identity requires a staff intermediary and careful separation of grades and study data.

**Challenges for adopters.**

- The workflow depends on PathMX or an equivalent handwriting-to-LaTeX tool.
- Students need access to an AI agent, which may involve licensing costs.
- Designing effective guardrails requires faculty time.
- Institutional AI policies vary and may constrain adoption.

## References

[1] Johnson, M., Alvin, C., [*Toward True Differentiated Instruction with PathMX and Curriculum as Code*](https://dl.acm.org/doi/10.5555/3820586.3820601), The Journal of Computing Sciences in Colleges, 2026, 41(8).

[2] Johnson, M., Le, T., Alvin, C., *An Agentic Authoring Continuum for Personalized Curriculum: Three Classroom Deployments*, *Proceedings of the 58th ACM Technical Symposium on Computer Science Education (SIGCSE TS 2027)*, Sacramento, CA, 2027.
