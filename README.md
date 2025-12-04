# QOF Indicator Lookup Tool

A simple, fast tool to find applicable Quality and Outcomes Framework (QOF) indicators for NHS GP practices in England.

## 🔗 Live Demo

**[Use the tool here](https://ninam-q.github.io/qof-indicator-tool/)**

## Features

- **Patient-based lookup**: Enter age, sex, and conditions to see all applicable QOF indicators
- **Smart grouping**: Indicators grouped by action type (Medications, Blood Pressure, Blood Tests, Reviews, etc.)
- **Medication checking**: Paste a patient's medication list to see which medication-related indicators are already met
- **Frailty & smoking status**: Toggle to see how indicators change based on frailty and smoking status
- **Consultation view**: Track which indicators are outstanding during a consultation
- **Offline capable**: Single HTML file with no dependencies - works without internet

## QOF 2025/26

This tool is based on the [QOF 2025/26 guidance](https://www.england.nhs.uk/publication/quality-and-outcomes-framework-guidance-for-2025-26/) from NHS England.

### Included Indicator Domains

**Clinical:**
- Atrial Fibrillation (AF)
- Ischaemic Heart Disease (CHD)
- Heart Failure (HF)
- Hypertension (HYP)
- Stroke & TIA (STIA)
- Peripheral Arterial Disease (PAD)
- Chronic Kidney Disease (CKD)
- Diabetes Mellitus (DM)
- Asthma (AST)
- COPD
- Dementia (DEM)
- Mental Health / SMI (MH)
- Non-diabetic Hyperglycaemia (NDH)
- Cholesterol & Lipid Management (CHOL)

**Public Health:**
- Blood Pressure screening (BP)
- Smoking (SMOK)
- Vaccinations & Immunisations (VI)
- Cervical Screening (CS)

## Usage

1. Enter patient's age (or age range if unknown)
2. Select patient's sex
3. Add relevant conditions
4. Optionally paste current medications
5. Set smoking and frailty status if known
6. Click "Find Applicable Indicators"

The tool will show all applicable QOF indicators grouped by action type, making it easy to work through systematically during a consultation.

## Smart Features

- **Superseding logic**: If a patient needs annual BP monitoring, the 5-yearly BP check is hidden (annual supersedes it)
- **Medication grouping**: Multiple indicators checking the same medication type are combined into one action
- **CVD history detection**: Automatically detects CVD history from selected conditions for primary/secondary prevention indicators
- **Unknown status handling**: When smoking or frailty status is unknown, shows both variants with amber highlighting

## Installation

No installation required! Simply:

1. Download `index.html`
2. Open in any modern web browser

Or use the hosted version via GitHub Pages.

## Contributing

Contributions welcome! Please feel free to submit issues or pull requests.

### Potential improvements:
- [ ] Add exception/exclusion code suggestions
- [ ] Export consultation checklist as PDF
- [ ] Add SNOMED code references
- [ ] Include indicator rationale from QOF guidance

## Disclaimer

This tool is provided for informational purposes only. Always refer to the official [QOF guidance](https://www.england.nhs.uk/publication/quality-and-outcomes-framework-guidance-for-2025-26/) and [business rules](https://digital.nhs.uk/data-and-information/data-collections-and-data-sets/data-collections/quality-and-outcomes-framework-qof) for definitive information.

## License

MIT License - feel free to use, modify, and distribute.

## Acknowledgments

- NHS England for the QOF guidance documentation
- Built with Claude (Anthropic)
