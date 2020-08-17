{
  "services": [
    {
      "id": "demo-suggestion-card",
      "hook": "patient-view",
      "title": "Bilirubin Sample Suggestion Card",
      "description": "Sends a Bilirubin Sample Suggestion Card"
    },
    {
      "id": "bilirubin-cds-hook",
      "hook": "patient-view",
      "title": "Bilirubin CDS Hooks ExecutableService",
      "description": "Detects issues with infants and the Kernicterus risk protocol",
      "prefetch": {
        "patient": "Patient/{{context.patientId}}",
        "observations": "Observation?patient={{context.patientId}}&code=http://loinc.org|58941-6&_sort:desc=date&_count=1"
      }
    },
    {
      "id": "demo-app-link-card",
      "hook": "patient-view",
      "title": "Bilirubin Sample Application Link Card",
      "description": "Sends a Bilirubin Sample Application Link Card"
    },
    {
      "id": "demo-info-card",
      "hook": "medication-prescribe",
      "title": "Hello World Med Prescribe Card",
      "description": "Sends a Hello World Info Card"
    }
  ]
}
