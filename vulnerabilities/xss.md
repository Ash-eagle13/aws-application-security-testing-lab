# Cross-Site Scripting (XSS)

## Description
Cross-Site Scripting occurs when an application allows untrusted input to be executed as JavaScript in a user's browser.

## Test Procedure

1. Navigate to search bar
2. Enter payload:

<script>alert('XSS')</script>

## Result

The payload executes a JavaScript alert, demonstrating that user input is not properly sanitized.

## Impact

An attacker could steal session cookies or execute malicious scripts.

## Mitigation

- Sanitize user inputs
- Implement output encoding
- Use Content Security Policy
