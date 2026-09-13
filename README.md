See the Project Plan of Deep Learning-Based Classification of Early and Late Blight in Potato Leaves for the initial phase of the project.
An executed research pipeline comparing logistic regression, a compact PotatoCNN and MobileNetV2. The package includes the source notebook, an exported Python pipeline, three trained models, recorded results, architecture, Assessment 1 and Assessment 2 reports, and named project-planning records.

Repository: [https://github.com/mahdihasan0017/PRT661-Data-Science-Practice-Dan-7-Theme-2](https://github.com/mahdihasan0017/PRT661-Data-Science-Practice-Dan-7-Theme-2)

## Start here

1. Read [Assessment requirements and status](ASSESSMENT_REQUIREMENTS.md).
2. Open the [28-page consolidated Assessment 2 PDF](assessment_reports/Assessment_2_Consolidated_Progress_Report.pdf).
3. Inspect the [executed notebook](notebooks/CODE.ipynb) and [saved model comparison](artifacts/tables/final_model_comparison.csv).
4. Run the dependency-free integrity check from this repository root:

```console
python scripts/validate_repository.py
```

For data acquisition, environment setup and execution, follow [REPRODUCIBILITY.md](REPRODUCIBILITY.md). No raw image dataset download is needed to inspect the saved evidence.

## Recorded results

| Model | Internal accuracy | External PlantDoc accuracy | Internal Late F1 | External Late F1 |
|---|---:|---:|---:|---:|
| Logistic regression | 91.00% | 48.65% | 0.9109 | 0.5043 |
| PotatoCNN | 95.33% | 51.35% | 0.9533 | 0.1290 |
| MobileNetV2 | 99.67% | 58.56% | 0.9966 | 0.4831 |

PlantVillage: 2,000 images / 500 leaf groups; 1,400/300/300 train/validation/test images and zero shared groups. PlantDoc: 222 external images. Late Blight is positive; thresholds are selected on validation only. See [internal](artifacts/tables/final_model_comparison.csv) and [external](artifacts/tables/plantdoc_external_metrics.csv) results. Strong controlled-source accuracy does not establish field reliability. The prototype has no Healthy/Other class and provides no diagnosis or treatment advice.

## Team

| Name | Student ID | Documented responsibility |
|---|---|---|
| Kavya Sree Sunkara | S386025 | Data acquisition and repository setup |
| Sayed Mahidul Islam Rafel | S387949 | Image preprocessing and exploratory analysis |
| Mahdi Hasan Abdullah | S394885 | CNN development and model training |
| Partha Mallik | S392819 | Evaluation, visualisation and error analysis |
| Datta Sai Kanaparthi | S385673 | Documentation, ethics review and final integration |

Roles come from the supplied [team structure](planning/team_structure_responsibilities.pdf). Allocations do not prove individual completion. See [authentic collaboration evidence](project_management/COLLABORATION_EVIDENCE.md).

## Repository layout

| Folder | Contents |
|---|---|
| `notebooks/` | Executed source notebook, preserved unchanged |
| `src/` | Python export of the same pipeline |
| `artifacts/models/` | Logistic joblib and two PyTorch state dictionaries |
| `artifacts/tables/` | Splits, audits, predictions and metric tables |
| `artifacts/figures/` | Experimental figures and Assessment 2 figure exports |
| `artifacts/documentation/` | Recorded environment, provenance and limitations |
| `architecture/` | Original/updated architecture, workflows and editable DOT sources |
| `assessment_reports/` | Original proposal, checked consolidated PDF and editable reports |
| `planning/` | Named team, plan, allocation and risks |
| `project_management/` | Tasks, milestones, proposed sprint plan and real evidence links |
| `data/` | Dataset acquisition and path guidance; no raw corpus included |
| `scripts/` | Static evidence/integrity validator |
| `evidence/individual/` | Named contribution pages and missing-evidence instructions |

## Submission status

The repository package is assembled and locally validated. It has not been uploaded by this packaging operation. Lab 1 screenshots, student-authored reflections, some individual evidence and a usable project-board URL still need the team's input. The latest user-edited Word document is included separately; the checked PDF predates those edits. See [report versions](assessment_reports/README.md) and [packaging changes](CHANGELOG.md).

## Licence and data terms

See [data and licensing notes](DATA_AND_LICENSES.md). No new licence grant is asserted for student work or trained models. Do not treat dataset source links as permission to redistribute raw images.
