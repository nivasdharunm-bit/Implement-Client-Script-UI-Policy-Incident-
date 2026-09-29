function onChange(control, oldValue, newValue, isLoading, isTemplate) {
    if (isLoading || newValue == '') {
        return;
    }

    if (newValue == '1') {
        g_form.setMandatory('subcategory', true);
    } else {
        g_form.setMandatory('subcategory', false);
    }
}
Incident Client Script & UI Policy
│
├── Client Scripts
│   ├── Incident - onLoad
│   ├── Incident - onChange
│   └── Incident - onSubmit
│
├── UI Policies
│   ├── Incident - Make Field Mandatory
│   ├── Incident - Show/Hide Field
│   └── Incident - Make Field Read Only
│
└── Testing
    ├── Test Client Script
    ├── Test UI Policy
    └── Verify Incident Form