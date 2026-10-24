# Handover card: UAT test data

**From:** Lina · **To:** Dana · **Date:** 17 March · **Version:** 1.0

## 1. In one sentence
The shared sheet of test patients, doctors and clinics that QA and the client use for every UAT session.

## 2. Why it matters
Without valid test data, UAT sessions stall in the first ten minutes and the client loses confidence.

## 3. State today
Up to date for release 2.3. A "missing" tab lists data we still need (two doctor accounts with expired licences).

## 4. How to run it
1. Before each UAT session, open the "next session" tab and check every account still logs in on staging.
2. Add anything new you create during testing to the right tab, same day.
3. Move used-up records (e.g. a booking that can't be cancelled twice) to "used".
4. Every Monday, send the "missing" tab to the QA lead.

## 5. Open items
| Item | Waiting on | Since | Next action |
|---|---|---|---|
| Two expired-licence doctor accounts | Backend team | 4 Mar | Chase on Thursday's stand-up |

## 6. People
| Who | Role | When to contact them |
|---|---|---|
| Rami | QA lead | Weekly "missing" list; failed logins |
| Backend team | Creates special accounts | Anything that can't be made through the UI |

## 7. Traps
- Staging is reset every second Sunday. Recheck logins on Mondays.
- Never copy production data into the sheet, even "just one record".

## 8. Access needed
The shared sheet (edit), staging portal (test user role), staging back office (QA role).

## 9. Keep, simplify or retire?
Keep. Lina suggests merging the "used" tab into the main tab with a status column. Dana to decide.

## 10. Checklist
- [x] Receiver read the card
- [x] Walkthrough done (date: 18 Mar)
- [ ] Receiver did the main task alone (date: )
- [ ] Access moved
- [x] Receiver's questions answered in this card
