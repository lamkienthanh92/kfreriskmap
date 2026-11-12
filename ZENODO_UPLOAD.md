# Manual upload to Zenodo: values for each field

Upload form: https://zenodo.org → "+" → New upload. Fields marked * are required.

## Before you start
1. Fill in Basic information, answer "No" to the DOI question and press **Get a DOI now!**. Copy the reserved DOI and press **Save draft**.
2. Replace `10.5281/zenodo.XXXXXXX` with the reserved DOI in `README.md`, `CITATION.cff` and `index.html`, then zip the folder again as `kfre-risk-map-v2.2.0.zip`.
3. Return to the draft and upload the zip. Files cannot be changed after publication.

## Files
- `kfre-risk-map-v2.2.0.zip`
- Optional: `assets/screenshot.png` as a second file, set as the default preview.

## Basic information
| Field | Value |
|---|---|
| Digital Object Identifier * | No → Get a DOI now! |
| Resource type * | Software |
| Title * | KFRE Risk Map: kidney failure risk against the KDIGO 2024 heat map |
| Publication date * | 2026-11-12 |
| Creators * | See table below, in the agreed author order |
| Description | See text below |
| Licenses * | Remove the default CC BY 4.0; add **MIT License** |
| Copyright | Copyright 2026 Nguyễn Thụy Trâm Anh, Lâm Hà Thu, Huỳnh Hoài Nam, Trần Nguyễn Thu Hiền, Lâm Kiến Thành, Lê Văn Chương |

### Creators
| # | Family name | Given names | Affiliation |
|---|---|---|---|
| 1 | Nguyễn | Thụy Trâm Anh | Lanh Binh Thang General Hospital |
| 2 | Lâm | Hà Thu | Lanh Binh Thang General Hospital |
| 3 | Huỳnh | Hoài Nam | Lanh Binh Thang General Hospital |
| 4 | Trần | Nguyễn Thu Hiền | Lanh Binh Thang General Hospital |
| 5 | Lâm | Kiến Thành | [affiliation] |
| 6 | Lê | Văn Chương | [affiliation] |

Add an ORCID iD for each person who has one.

### Description
Browser-based companion tool to a cross-sectional study of 129 outpatients with chronic kidney disease (CKD) G3–G5 at Lanh Binh Thang General Hospital, Ho Chi Minh City, Vietnam. It calculates 2- and 5-year kidney failure risk with the 4-variable Kidney Failure Risk Equation (non-North American and North American calibration) and sets the result against the KDIGO 2024 eGFR–albuminuria heat map. The tool shows iso-risk contours on the eGFR–ACR plane, the KDIGO 2024 action thresholds next to the corresponding eGFR criteria, a decomposition of the estimate from the KFRE reference patient, what-if curves, and the stability of threshold classification on simulated repeat testing.

Run it by opening index.html in a browser; no installation or build step is needed.

Research and education tool; not a medical device. The KFRE has not been validated in Vietnamese patients.

## Recommended information
| Field | Value |
|---|---|
| Keywords | chronic kidney disease; kidney failure risk equation; KDIGO 2024; risk stratification; clinical decision support; Vietnam |
| Languages | English |
| Version | 2.2.0 |
| Publisher | Zenodo (default) |

## Software
| Field | Value |
|---|---|
| Repository URL | https://github.com/YOUR-USER/kfre-risk-map (if published on GitHub) |
| Programming language | JavaScript |
| Development status | Active |

## Related works (after the article is published)
Relation "Is supplement to", the article DOI, resource type "Publication / Journal article".

## References
Paste the six references listed in README.md, one per line.

## Visibility
Full record: Public. Files: Public (or remove `assets/js/cohort.js` first if publication of the clinic data is not covered by the ethics approval).

Save draft → Preview → Publish.
