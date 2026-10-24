# Note triage guide

After a UAT, sprint review or client session you have a pile of notes. Before anything goes to the backlog, sort each note into exactly one class, checked against the **baseline**: the signed requirements (SRS, user stories, approved screens).

## The classes

| Class | Test | Goes to |
|---|---|---|
| **Bug** | The system does not do what the baseline says | Development, as a defect |
| **Tweak** | Small change inside the baseline's intent (wording, label, order, a missing validation the baseline implies) | Development, low effort |
| **Change request (CR)** | The client wants something the baseline does not say, or says differently | CR process: impact analysis, estimate, client approval **before** any work |
| **Duplicate** | Same as an existing item | Link to the existing item |
| **Not an issue** | Works as specified; the note is a misunderstanding | Reply to the client with the baseline reference |
| **Needs clarification** | You can't decide without asking | Question to the client, with an owner and a date |

## How to decide (in this order)

1. Is it already logged? → **Duplicate**.
2. Find the baseline item. None exists? → **CR** (or **Needs clarification** if unsure).
3. Does the system match the baseline? No → **Bug**.
4. It matches, but the client wants it different → small and within intent → **Tweak**; otherwise → **CR**.
5. It matches and the client misunderstood → **Not an issue**.

## For every CR, write the impact

- Which screens, services, integrations, reports and documents it touches.
- Effort estimate and effect on the timeline.
- Who must approve it.

## Why it matters

Treating CRs as bugs makes development look slow and hides scope growth. Treating bugs as CRs makes the client pay for your defects. The baseline check is what keeps both sides fair.

## Using an AI assistant

An LLM is good at a first pass: matching a note to the closest baseline item and proposing a class. Keep a human decision on every note, and never paste confidential client data into a tool your organisation hasn't approved.
