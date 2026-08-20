# GitHub repo — what to fill in

Created with no README, no licence, no .gitignore — correct, the repo
already has all three and letting GitHub generate them makes the first push
conflict.

## Description (the one-liner under the repo name)

```
A QA layer for AI-drafted clinical notes: decomposes each note into individually checkable claims, verifies every one against the source transcript, and flags anything unsupported for human review before a clinician signs.
```

219 characters, well inside GitHub's 350 limit. It says what it does and who
it is for without needing the reader to already know what an ambient scribe
is.

## Website field

```
https://clinicalnoteguard.netlify.app
```

Easy to miss and worth more than the description — it puts a clickable link
to the working demo at the top right of the repo page, which is the first
thing a judge who opens the repo will see.

## Topics

Lowercase and hyphenated, GitHub allows up to 20:

```
llm  prompt-engineering  hallucination-detection  healthcare  clinical-nlp
evaluation  llm-evaluation  ambient-scribe  python  gemini  groq
human-in-the-loop  hackathon
```

## Then push

```
git remote add origin https://github.com/Gurneil/Clinical-Note-Guard.git
git push -u origin master
```

Your default branch will be `master`, not `main`. Renaming this close to a
deadline is a needless risk and nobody judging will care.

## Before you consider it done

- [ ] Confirm `.env` is NOT in the repo. It is gitignored and was never
      committed on any branch — verified — but look at the file list once
      with your own eyes, because this is the one mistake that cannot be
      undone by deleting it later.
- [ ] The site's "View on GitHub" button starts working the moment the repo
      is public. Click it.
- [ ] Older commits are authored `Geel <samuelclaude9000@gmail.com>`. To have
      GitHub attribute them to you, add that address as a secondary email in
      Settings → Emails.
