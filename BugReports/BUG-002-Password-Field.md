# BUG-002 - Password Field Accepts Leading Spaces

## Summary

Password field accepts leading spaces and processes them as valid characters.

## Environment

* Application: OrangeHRM Demo
* Browser: Google Chrome

## Severity

Low

## Priority

Low

## Preconditions

User account exists.

## Steps to Reproduce

1. Open Login page.
2. Enter valid username.
3. Enter password with leading spaces.
4. Click Login.

## Expected Result

System should trim leading spaces or show validation.

## Actual Result

System accepts input including leading spaces.

## Status

Open

## Reporter

Mustafa Konu
