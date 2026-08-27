# Dataset Provenance

This file documents the origin, identifiers, and access information for the
three CT datasets used to build the anatomical models in this repository
(s0011, s0024, MIDRC), as well as the segmentation tools used, to support
reproducibility.

## Model: MIDRC

| Category | Field | Value |
|---|---|---|
| Identification | Case ID | 10000364-6553460 |
| | Object ID | dg.MD1R/6052a7a3-e477-48a2-9119-efe296bd68dc |
| | Project | Open-A1 |
| | Data source | ct_series_file |
| | Data contributor | ACR |
| | Data format | DICOM (.dcm) |
| | Data category | CT |
| Patient data | Sex | Male |
| | Age at index event | 54 years |
| | Race | Black or African American |
| | ZIP code | 0 (anonymized) |
| Imaging study | Modality | CT |
| | Series description | PV 1.25 |
| | Study description | CT CHEST ABDOMEN PELVIS W CONTRAST (ROUTINE) |
| | Number of images (instances) | 529 |
| | Manufacturer | GE Medical Systems |
| | Scanner model | Revolution CT |
| | Series UID | 2.16.840.1.114274.1818.570651552348430371917403886355416247 |
| | Study UID | 2.16.840.1.114274.1818.462575414143272543913985841241130676639 |
| COVID-19 | COVID-19 positive | Yes |
| | Index event | COVID-19 test |
| | Days from study to positive test | +30 days |
| | Days from study to negative test | +274 days |
| | Study year shifted | Yes (for privacy) |
| LOINC | LOINC code | 72254-6 |
| | LOINC long name | CT Chest and Abdomen and Pelvis W contrast IV |
| | LOINC method | CT |
| | LOINC anatomical system | Chest + Abdomen + Pelvis |
| | Contrast (LOINC) | With intravenous contrast |
| Additional | Official citation | 2024: ACR_20211115. dg.MD1R/6052a7a3-e477-48a2-9119-efe296bd68dc |
| | MD5sum (file verification) | d4a65917d5b585aca6e55c4061c8c1f2 |
| Access | Source | MIDRC Data Commons Explorer: https://data.midrc.org/explorer |
| | License / access terms | Available through the MIDRC Data Commons (registration/data use agreement required), supported by NIBIB under contract 75N92020D00021 and ARPA-H |

## Model: s0011

| Category | Field | Value |
|---|---|---|
| Identification | Source dataset | TotalSegmentator Dataset v2.0.1 |
| | Case/folder ID | s0011 (as provided in the downloaded dataset) |
| | Access method | Downloaded via MATLAB |
| Patient data | Anonymized | Yes; no demographic metadata available |
| Imaging study | Number of images (instances) | 431 |
| | Slice thickness / spacing | 1.5 mm |
| | Contrast | None |
| | Anatomical coverage | T1-Sacrum |
| Access | Source | https://zenodo.org/records/10047292 |
| | License | CC BY 4.0 |

## Model: s0024

| Category | Field | Value |
|---|---|---|
| Identification | Source dataset | TotalSegmentator Dataset v2.0.1 |
| | Case/folder ID | s0024 (as provided in the downloaded dataset) |
| | Access method | Downloaded via MATLAB |
| Patient data | Anonymized | Yes; no demographic metadata available |
| Imaging study | Number of images (instances) | 486 |
| | Slice thickness / spacing | 1.5 mm |
| | Contrast | None |
| | Anatomical coverage | T1-Sacrum |
| Access | Source | https://zenodo.org/records/10047292 |
| | License | CC BY 4.0 |

## Software / Segmentation Tools

| Tool | Version/Reference | License | Role in this project |
|---|---|---|---|
| MONAI Auto3DSeg (3D Slicer extension) | Last updated December 15, 2024 | - | Automatic segmentation (Vertebrae/Muscles/Whole body TS2-quick configs) |
| TotalSegmentator v2 (pretrained models) | Wasserthal et al. (2023), *Radiology: Artificial Intelligence*, DOI: 10.1148/ryai.230024. Repository: https://github.com/wasserth/TotalSegmentator | Apache-2.0 | Underlying models used by MONAI Auto3DSeg's "TS2-quick" configurations |
