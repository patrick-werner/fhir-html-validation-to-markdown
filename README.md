# Convert FHIR HTML Validation Reports to Markdown
Action to convert the html output of the java fhir validator to markdown

Usage

To use this action in your GitHub workflow, add the following to your .github/workflows/your-workflow.yml:

```yaml
jobs:
  convert-validation:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - name: Convert Validation Report
        uses: patrick-werner/fhir-html-validation-to-markdown@1.0.0-alpha1
        with:
          input_file: './path/to/validation.html'
```
