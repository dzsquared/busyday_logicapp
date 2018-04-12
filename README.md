# busyday_logicapp
Azure Logic App for Managing Upcoming Busy Days

**The logic app will check your calendar for the next week and on any days with 4 or more meetings, add a full day appointment as a reminder to yourself and others to avoid scheduling anything else into that busy.**

## Implement in your Azure Portal
- The logic app connects to an Office 365 mailbox, which is designated by "office365" in the json.  Input your own connectionid and id.
- The calendar where the full day appointment is being placed is selected by id, which will need to be populated.  This can be selected in the designer once the logic app is connected to Office 365.
- hourstoaddTZ and hoursplus19TZ are adjusted from UTC to CST by reducing the original values by 6 (hourstoadd vs hourstoaddTZ and hoursplus19 vs hoursplus19TZ).