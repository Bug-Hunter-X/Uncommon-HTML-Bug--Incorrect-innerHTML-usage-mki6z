# Uncommon HTML Bug: Incorrect innerHTML Usage

This repository demonstrates a subtle but potentially problematic error related to using `innerHTML` in HTML.  The example shows how incorrectly using `innerHTML` to add multiple HTML elements can lead to unexpected behavior and even open security vulnerabilities.

## The Bug
The primary issue is that directly adding complex HTML structures using `innerHTML` bypasses the browser's parsing and DOM manipulation mechanisms, potentially leading to unexpected DOM tree structures. Further, it creates a significant XSS vulnerability because the injected content is directly interpreted as HTML.