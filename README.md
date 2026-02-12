# Exploring Security Center Hardening and Best Practices

## Overview
This repository demonstrates the implementation and validation of instance hardening and security best practices using the ServiceNow Security Center. The focus is on reviewing hardening compliance scores, modifying non-compliant security settings, and validating best practice task completion.

This project simulates how an administrator evaluates instance security posture, applies configuration changes, and tracks compliance improvements using Security Center.

## Use Case
An administrator is responsible for improving the security posture of a ServiceNow instance. The administrator must review the current hardening compliance score, remediate high-impact non-compliant settings, and validate progress through the Security Center Best Practices dashboard.

This project simulates how ServiceNow Security Center provides visibility into configuration risk areas and enables guided remediation of security settings.

## Features
- Security Center overview dashboard review
- Hardening compliance score comparison
- Identification of non-compliant security settings
- Configuration of password policy enforcement
- Modification of session timeout duration
- Compliance validation through updated score tracking
- Best Practices task review and completion tracking

## Technologies Used
- ServiceNow Platform
- Security Center
- Security Configuration Console
- System Properties
- Instance Hardening Settings
- Compliance Scoring
- Best Practices Dashboard

## Implementation Walkthrough

### Objective
Review instance hardening compliance, remediate non-compliant security settings, and validate configuration updates using Security Center.

### Step 1: Navigate to Security Center
The Security Center was accessed by navigating to **All > Admin Center > Security Center**.

The landing page displayed the Security configuration console overview.

### Step 2: Review Hardening Score Comparison
Within the Tools section, **Security Configuration > Hardening score comparison** was selected.

The hardening compliance score was reviewed, showing an example score of 89%. The comparison displayed score values across two dates.

This provided visibility into the current security compliance posture.

<img width="1907" height="361" alt="Screen Shot 2026-02-11 at 8 31 36 PM" src="https://github.com/user-attachments/assets/a6cfcd22-baf5-4bc5-8de4-66a49f4739b5" />

### Step 3: Access All Hardening Settings
The **All settings** option was selected to review all hardening configurations.

The dashboard displayed compliant and non-compliant setting counts.

### Step 4: Review Non-Compliant Settings
The **Non-compliant settings** tile was selected.

The list displayed high-priority non-compliant settings, including score impact and security category.

This identified which configurations would most improve the compliance score.

### Step 5: Enforce Current Password Policy Compliance
The hardening setting **Enforce Current Password Policy Compliance Requirements on Login** was selected.

Within the Setting configuration section, the property `glide.apply.password_policy.on_login` was modified by enabling the Current configuration toggle.

The configuration was updated to apply the change.

This action moved the setting toward compliance.

<img width="1907" height="839" alt="Screen Shot 2026-02-11 at 8 40 17 PM" src="https://github.com/user-attachments/assets/7eb13e7e-c0d3-47fd-abca-d42d0fd01d0c" />

### Step 6: Modify Session Timeout Duration
The list of non-compliant settings was revisited and **Minimize Session Activity Timeout Duration** was selected.

Within the Setting configuration section, the `glide.ui.session_timeout` property was modified from the default value of 1445 to 60.

The configuration was updated to apply the change.

This ensured session inactivity timeout aligned with recommended security standards.

<img width="1907" height="808" alt="Screen Shot 2026-02-11 at 8 38 50 PM" src="https://github.com/user-attachments/assets/48438f16-a66b-4979-802f-9d9df2d2a691" />

### Step 7: Validate Compliance Updates
The **Compliant settings** view was selected.

The Updated column was added to the list view and sorted in descending order.

Both updated settings were confirmed as compliant, indicated by the green compliance flag.

This validated that configuration changes were successfully applied.

<img width="1907" height="664" alt="Screen Shot 2026-02-11 at 8 46 50 PM" src="https://github.com/user-attachments/assets/12fb0388-87f9-494e-8515-f687e2aa86a6" />

### Step 8: Navigate to Security Posture
From the Security Center overview, the Tools section was accessed and **Security posture** was selected to browse Best Practices.

The Best Practices dashboard displayed maturity levels and available recommendations.

### Step 9: Select Build a Foundation
The **Build a foundation** maturity level was selected.

The lower section of the screen displayed tasks associated with this maturity track.

### Step 10: Review Default Login Credential Recommendation
The Best Practice **Change the default login credentials** was selected.

The task details were reviewed.

The **Go to next step** option was selected to view task progress.

### Step 11: Mark Best Practice as Complete
Under Task Steps, **Change the default login credentials** was expanded.

For this scenario, the step was marked complete by selecting **Mark Step Complete**, followed by **Complete Best Practice**.

The task status was updated to reflect completion.

<img width="1907" height="515" alt="Screen Shot 2026-02-11 at 8 50 43 PM" src="https://github.com/user-attachments/assets/e710178a-1972-4af8-befd-20e967218765" />

### Step 12: Validate Best Practices Dashboard Progress
The Best Practices landing page was revisited.

The Completed overall count displayed progress, confirming that the first best practice step was successfully completed.

This validated that Security Center tracked configuration and best practice activity accurately.

## Validation and Testing

### Step 13: Confirm Hardening Compliance Changes
The Hardening compliance score was reviewed to confirm that configuration updates were reflected in the system.

Both password policy enforcement and session timeout duration were marked compliant.

### Step 14: Confirm Best Practice Completion
The Best Practices dashboard displayed updated completion metrics.

The progress indicator reflected one completed task under the selected maturity track.

This confirmed successful interaction with both hardening settings and Best Practice workflows.

<img width="1907" height="357" alt="Screen Shot 2026-02-11 at 8 51 29 PM" src="https://github.com/user-attachments/assets/39483c72-ec70-4fbf-afd1-a6fb77cf9ea2" />

## Lessons Learned
- Security Center provides centralized visibility into instance hardening posture  
- Compliance scoring highlights high-impact configuration gaps  
- System properties directly influence security compliance  
- Hardening settings can be modified without custom scripting  
- Best Practices dashboards guide administrators through structured security improvements  
- Compliance updates are reflected immediately in configuration status tracking  
