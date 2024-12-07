# Unexpected CSS :focus-visible Override by :focus

This repository demonstrates an uncommon CSS issue where the `:focus-visible` pseudo-class is unexpectedly overridden by the `:focus` pseudo-class in certain browser environments.  This can lead to inconsistent styling when an element receives focus.  The provided code examples show the problem and a potential solution.

## Problem
The primary issue lies in the interaction between `:focus` and `:focus-visible`. The expectation is that `:focus-visible` styles should only be applied when focus is visible (e.g., by keyboard or mouse click interaction), allowing for more nuanced control over focus indicators.  However, in some cases, the `:focus` styles completely supersede the `:focus-visible` styles, regardless of how focus is obtained. 

## Solution
The proposed solution involves a more careful ordering and specificity of CSS rules, potentially adjusting selectors to ensure the desired behavior is consistently applied across different browsers and situations. More robust solutions sometimes involve JavaScript to manually handle focus events.