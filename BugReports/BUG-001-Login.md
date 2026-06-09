# BUG-001 - Login Button Remains Enabled When Mandatory Fields Are Empty

## Summary

Login button remains clickable even when Username and Password fields are empty.

## Environment

* Application: OrangeHRM Demo
* Browser: Google Chrome
* Version: Latest

## Severity

Medium

## Priority

Medium

## Preconditions

User is on the Login page.

## Steps to Reproduce

1. Open Login page.
2. Leave Username field empty.
3. Leave Password field empty.
4. Click Login button.

## Expected Result

System should disable Login button or display validation messages before submission.

## Actual Result

Login request is submitted even though mandatory fields are empty.

## Status

Open

## Reporter

Mustafa Konu
