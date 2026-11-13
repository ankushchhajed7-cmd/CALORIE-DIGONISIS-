# Calorie Diagnosis — STATE

**Current version:** v1.27 (13-11-2026) · branch `feature-v1.27` (main par abhi v1.26)
**Live link:** https://ankushchhajed7-cmd.github.io/CALORIE-DIGONISIS-/
**Owner:** Ankush New Vision · APK: `apk-factory` repo (`.github/workflows/build-apk.yml`)

## Files (GitHub mein yahi naam)
| File | Kaam |
|---|---|
| index.html | Poora app (ek file, vanilla JS) |
| sw.js | Service worker, network-first, cache `calorie-diagnosis-v1.27` |
| manifest.json | PWA; theme_color #1F6B4F (dark hi rakhna — APK license page isi se padhta hai) |
| icon-192.png, icon-512.png | Patti wala logo |
| STATE.md | Yeh file |

QR poster aur preview.png GitHub par nahi daalne.

## Settings / faisle (decisions)
- AI key customer khud banata hai (Gemini default `gemini-3.6-flash`, Claude option). Key lock, kabhi hatati nahi. License APK Factory karta hai (app ke andar nahi).
- Poore din ka AI plan: din mein 1 baar (raat 12 baje khulta). Ek dish 30 din mein max 3 baar.
- **Aage ka plan (v1.27):** khaye hue ke baad baaki din. Offline plan hamesha; AI wala din mein 3 baar tak (`cd_restplan`), poore din wale lock se alag.
- Bachi calorie = target + walk bonus (jali calorie ka aadha) − khaya.
- Bhasha: Hindi (देवनागरी) default, Hinglish, English. Har naya text EN + HI dictionary mein.
- Data localStorage + IndexedDB; roz auto backup file; naye install par backup restore.
- Report raat 8 baje ke baad (REPORT_HOUR=20).
- Kidney problem ho to potassium/protein "kam hai" wali salah band.

## Version history
- v1.27 (13-11-2026): "Aage ka plan" — jo khaya uske baad baaki din ka plan
- v1.26 (25-09-2026): Backup chunte waqt salah — "file na dikhe to ☰ menu → Downloads"; restore mein har tarah ki file chun sakte ho
- v1.25 (25-09-2026): Settings mein APK jaanch — camera / step sensor / permission ki haalat saaf likhi
- v1.24 (25-09-2026): APK mein phone ke step-counter chip se kadam apne aap (app band ho tab bhi chip ginta hai)
- v1.23 (25-09-2026): Khaya hua item badlo — item par tap: ¼ / ½ / ¾ / poora / 1½ / 2, −/+, ya calorie khud likho;
- v1.22 (25-09-2026): App ka QR code — welcome screen par (tap karo to bada), Settings → Madad mein "App share karo (QR)"; Share / WhatsApp button
- v1.21 (25-09-2026): Ek hi photo = ek hi calorie
- v1.20 (25-09-2026): Naye install par "📂 Purana backup wapas laao" — welcome screen aur pehle sawaal par
- v1.19 (25-09-2026): Purana APK pehchano — camera button par "naya APK banao" ki salah (Settings mein APK version bhi)
- v1.18 (25-09-2026): APK mein walk ke time screen on (naye APK Factory ke ANVScreen se)
- v1.17 (25-09-2026): Back button + walk sensor sudhaar
- v1.16 (25-09-2026): Asli Hindi (देवनागरी)
- v1.15 (25-09-2026): Icon jaisa halka hara Light theme
- v1.14 (25-09-2026): Welcome dashboard + walk / steps
- v1.13 (25-09-2026): English option + app ki din ki report
- v1.12 (25-09-2026): Naya saaf layout + app guide + dawai / allergy
- v1.11 (25-09-2026): Profile ke liye ek-ek sawaal (Stage 1: wazan kam karna)
- v1.10 (24-09-2026): v1.07 se aage (v1.08 ka in-app license hataya — license ab APK Factory karega)
- v1.07 (24-09-2026): Key guide page + key lock + daily auto backup
- v1.06 (24-09-2026): AI button = har baar naya 1 din ka plan
- v1.05 (24-09-2026): AI plan har din alag
- v1.04 (24-09-2026): Problem chart (6 point)
- v1.03 (23-09-2026): Busy-server fix + target box check
- v1.02 (23-09-2026): Gemini model fix
- v1.01 (23-09-2026): Poshan tracking
- v1.00 (23-09-2026): Pehla build

## Pending / aage
- Naya APK (1.21+) banana zaroori: camera capture, step-chip (ANVSteps), screen-on (ANVScreen).
- iPhone: APK nahi chalta — Safari "Add to Home Screen" se PWA.
- Idea: aage ka plan WhatsApp share mein bhi jodna (abhi share button poore din wala plan bhejta hai).
