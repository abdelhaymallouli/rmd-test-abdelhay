# tools/

This folder is intentionally minimal in the public template repo.

The auto-grader for the QCM (`grade-qcm.py`) and the canonical answer key (`answer-key.json`) live in a **separate, private** repository: `RMDCreations/rmd-recruitment-graders`.

This separation exists so the public template repo can be safely cloned, forked, or re-used for future cohorts without leaking the answer key.

If you are a **candidate** reading this: nothing for you to do here. Move on to the section briefs.

If you are an **RMD reviewer** reading this: clone the private grader repo and run:

```bash
python grade-qcm.py path/to/candidate/01-qcm/answers.json
```
