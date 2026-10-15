# Windows Security Log Investigation — Mock Incident Report

## 1. Objective

Investigate Windows Security event logs in a controlled Windows Server 2025 virtual lab to understand how authentication failures are recorded and assessed.

## 2. Environment

* Operating system: Windows Server 2025
* Virtualization: Oracle VirtualBox
* Log source: Windows Security event log
* Investigation type: Controlled lab exercise
* Production systems involved: No

## 3. Observed Event

* Event ID: 4625
* Date and time: 10/14/2026 11:26:27 PM
* Account name: Sally
* Failure reason: Unknown username or bad password
* Logon type: 2
* Source address: 127.0.0.1

## 4. Investigation Steps

1. Opened Event Viewer and navigated to Windows Logs > Security.
2. Filtered or reviewed events to locate the relevant authentication activity.
3. Inspected the event details and recorded the available fields.
4. Compared the event's timestamp and details with the known lab activity, where applicable.

## 5. Findings

A failed authentication event was recorded in the Windows Security log. The event details were reviewed and compared with the controlled lab activity. 

## 6. Assessment

The observation demonstrates that the configured auditing captured this test event. No conclusion about malicious activity was made.

## 7. Recommended Next Steps

Review related Windows Security events to determine whether other failed or successful authentication attempts occurred around the same time. Verify the account and examine available event details, such as the logon type, failure reason, and source address, if recorded. Correlate the event with known lab activity before drawing conclusions. In a real environment, escalate suspicious or unexplained activity according to the organization's incident response procedures.

## 8. Outcome and Lessons Learned

Successfully located and reviewed a failed authentication event in the Windows Security log. Learned how Windows Event Viewer can be used to examine authentication activity and how audit settings affect the events available for investigation. This exercise also demonstrated the importance of documenting observed evidence, distinguishing verified facts from assumptions, and identifying information that is unavailable. The investigation was limited to a controlled Windows Server 2025 virtual lab and did not establish malicious activity.
