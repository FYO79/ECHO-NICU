# WCH NICU Echo Forms – same idea as the NICU Duty Sheet

Upload to GitHub (replace the old files): `index.html`, `sw.js` (now `nicu-echo-v7`), `manifest.webmanifest`, `icon-192.png`, `icon-512.png`, `icon-800.png`.
Data stays on the device (localStorage). Babies saved in the old single-patient version (v6) open automatically as the first baby.

## Update 1 (sw v7) – NICU Duty style
- One tab per baby at the top (named by patient name, ID underneath) with **+ Baby**; each baby keeps its own PDA / PPHN / HYPOTENSION forms.
- **Echo summary (copy)** card: *Copy this form* or *Copy all three forms* gives a text report (patient data, filled findings, scores, conclusions) for the chart or WhatsApp. The text box shows what will be copied.
- **Send / save backup** (share sheet / AirDrop or a .json file) and **Receive / restore** to move all babies to another device.
- **Delete this baby**. Clear form clears only the open form.

## Earlier (v1–v6)
WCH branding; PDA = WCH shunting score only; PPHN and hypotension (Elsayed and Abdul Wahab 2021) automatic scores; respiratory settings by mode; automatic LVO/RVO, SVR, PASP.

## Update 2 (sw v8)
- Patient: Name / ID / Sex in one row; Date of birth / GA / Study date in one row; Birth and Current weight in one row. **Current weight is used in all calculations** (LVO, RVO, DO2); a reminder shows if it is blank.
- SpO2 pre-ductal, post-ductal and heart rate share one row.
- Cardiac structures: **Echo reviewed with cardiologist** (No / Yes); Yes opens name and date boxes.
- PDA shunting score table rearranged: equal-height rows, the scored column is highlighted, LVO inputs (Ao VTI, valve diameter) on their own line.
- PPHN / Hypotension: TR as **Measured TR (mmHg) and Estimated PAP (mmHg = TR + RAP)**; TR Vmax and gradient convert both ways. PAAT/RVET ratio has its own automatic box.
- IVC: optional max / min / aorta measurement gives collapsibility % and IVC/Ao. There is no validated neonatal cut-off for dilated or collapsed and the WCH forms give none; the single small study used is cited in the app.
- **Report** card (each form): findings, interpretation, recommendation, and a comparison table with the previous exam. Copy report, Copy all three forms, Print report.
- **New exam for the same baby:** change the Study date. Patient data stay; the exam fields start blank, and the report compares with the earlier exam (choose another with "Compare with"). Exam dates appear as buttons under the baby tabs.
- Data format changed: babies saved in v7 are not carried over.
