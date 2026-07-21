# LER DeltaGuard

AI revenue assurance for hospital billing. DeltaGuard scans operative notes against
the 2026 CMS coding changes for lower-extremity revascularization (LER) procedures,
flags under-coded cases with dollar-level deltas, and keeps medical coders in
control — every recommendation reviewed, every dollar traceable.

https://github.com/user-attachments/assets/f745c774-cb11-4679-876f-d0418459aee8


## How it works
1. **Upload** — hospital exports billing data + operative notes as CSV
2. **Scan** — the engine reads op notes for coding patterns against the 2026 LER framework
3. **Review** — flags surface with suggested CPT direction, projected delta, and confidence; coders accept or reject with comments
4. **Recover** — audit-ready export with exact dollar amounts and full reasoning trail

## Results
- 67 cases validated · 0 false positives · 0 missed catches
- $17,910 projected recovery on the stress-test dataset
- Identified via provider interviews + CMS data analysis (~$480M hospital revenue gap)
- 3rd place, Temple University startup pitch competition

## Architecture
Serverless AWS: Lambda, S3, API Gateway — projected compute costs cut ~90% vs. a
provisioned design. 

## Built by
Colin Fehlinger — https://www.linkedin.com/in/colin-fehlinger · colin.fehlinger@gmail.com
