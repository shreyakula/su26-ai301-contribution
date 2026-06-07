# Contribution 1: Add warning on the web interface stating the discussions aren't shared

**Contribution Number:** 1  
**Student:** Shreya Akula  
**Issue:** https://github.com/MISP/MISP/issues/3181  
**Status:** Phase I — Complete

---

## Why I Chose This Issue

I chose this issue because it's a clear, well-scoped UI improvement with 
obvious acceptance criteria. MISP is a threat intelligence platform, and 
users interacting with the discussions feature may not realize their 
conversations aren't shared across connected MISP instances — which could 
cause real confusion in security workflows. Adding a visible warning 
directly addresses that gap.

This issue is a good fit for my skills because the fix lives in the web 
interface, which means working with HTML/JavaScript in a real production 
codebase. I'm comfortable with frontend work and have experience building 
UI features and adding user-facing feedback in React projects. I'm excited 
to learn how MISP structures its PHP/JS frontend and to ship something that 
directly improves the user experience for security professionals.

---

## Understanding the Issue

### Problem Description

MISP has a discussions feature where users can post and reply to threads. 
However, these discussions are local to each MISP instance and are not 
shared with other connected instances. There is currently no warning or 
notice in the UI telling users this, which could lead to confusion about 
why their discussions aren't visible to peers on other instances.

### Expected Behavior

A clear warning or notice should appear somewhere in the discussions UI 
informing users that discussions are not shared across MISP instances.

### Current Behavior

No warning exists. Users have no way of knowing from the interface itself 
that discussions are instance-local.

### Affected Components

- The discussions web interface (likely a PHP template in the MISP views 
directory)
- Possibly a JavaScript component depending on how the UI is rendered

---

## Reproduction Process

### Environment Setup

[To be filled in during Phase II when I set up the local environment]

### Steps to Reproduce

1. Navigate to the discussions section in the MISP web interface
2. Observe that there is no warning about discussions not being shared
3. A user unfamiliar with MISP's architecture would have no way of knowing 
this limitation

### Reproduction Evidence

- **Commit showing reproduction:** [To be added in Phase II]
- **Screenshots/logs:** [To be added in Phase II]
- **My findings:** [To be added in Phase II]

---

## Solution Approach

### Analysis

[To be filled in during Phase II after reading the relevant template files]

### Proposed Solution

Add a visible warning message or banner to the discussions UI that clearly 
states discussions are not shared with other MISP instances. This will 
likely involve editing a PHP template file and possibly adding a styled 
alert component consistent with MISP's existing UI patterns.

### Implementation Plan

Using UMPIRE framework (adapted):

**Understand:** The discussions UI has no warning that discussions are 
instance-local. Users need to be informed of this limitation directly 
in the interface.

**Match:** [To be filled after reading how existing warnings/alerts are 
displayed elsewhere in the MISP UI]

**Plan:**
1. Set up local MISP environment
2. Find the relevant PHP template for the discussions view
3. Identify how existing alerts/warnings are styled in the codebase
4. Add a warning message consistent with MISP's UI patterns
5. Verify the warning appears correctly in the discussions interface

**Implement:** [Branch/commit links to be added as I work]

**Review:** [Self-review checklist to be added in Phase III]

**Evaluate:** Navigate to discussions, confirm warning is visible and 
styled correctly

---

## Testing Strategy

### Manual Testing

- [ ] Warning message appears on the discussions page
- [ ] Warning is styled consistently with other MISP UI alerts
- [ ] Warning does not break any existing discussions functionality
- [ ] Tested in local MISP environment

### Unit Tests

[To be determined after reviewing the project's existing test patterns]

---

## Implementation Notes

[To be filled in during Phase III as I build]

---

## Pull Request

**PR Link:** [To be added in Phase IV]  
**PR Description:** [To be drafted in Phase IV]  
**Maintainer Feedback:** [To be logged as received]  
**Status:** Not yet submitted

---

## Learnings & Reflections

[To be filled in after the contribution is complete]

---

## Resources Used

- [To be added as I work]
