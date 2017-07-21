# Jira Linker

A single-page application that transforms text with Atlassian JIRA ticket references to web link, pointing to the list of these tickets in JIRA.

## Use cases

Listing all JIRA tickets contained in some (part of) document (changelog, meeting notes, ticket description, git commit log, etc.), spreadsheet (plan, report, etc.), presentation or any other source that can be copied to clipboard and pasted as text.

## Example input

Version 1.4:
 * Implemented data export to JSON (APP-1010)
 * Fixed buffer overflows (APP-1015, APP-1017)

## Example output

```html
<a href="http://jira.example.com/issues/?jql=key%20in%20(APP-1010%2CAPP-1015%2CAPP-1017)">Your JIRA link</a>
```

## Features

 - Single HTML file with no external dependencies.
 - Stores JIRA URL and ticket prefix in localStorage.

## License

MIT License
