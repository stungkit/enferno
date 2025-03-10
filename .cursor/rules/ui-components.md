# UI Components and Patterns

## Vuetify Components
- Use Vuetify components for UI
- Leverage Material Design principles
- Keep styles minimal and use Vuetify's built-in classes

## Material Design Icons
- Use Material Design Icons for consistent iconography
- Reference icons with the `mdi-` prefix
- Example: `<v-icon>mdi-account</v-icon>`

## Data Tables
- Use the headers pattern for data tables
- Example:
```javascript
headers: [
    {title: 'ID', value: 'id'},
    {title: 'Name', value: 'name'},
    {title: 'Description', value: 'description', sortable: false},
    {title: 'Actions', value: 'actions', sortable: false}
]
```

## Forms and Dialogs
- Use the edialog pattern with eitem object for forms
- Example:
```javascript
edialog: false,
eitem: {
    id: "",
    name: "",
    description: ""
}
```

## Navigation
- Use the drawer pattern for navigation
- Example: `drawer: true`

## User Feedback
- Use the snackbar pattern for user feedback
- Example:
```javascript
methods: {
    showSnack(message) {
        this.snackMessage = message;
        this.snackBar = true;
    }
}
```

## Data Refresh
- Use the refresh pattern for data updates
- Call refresh after operations that modify data
- Example: `this.refresh()` 