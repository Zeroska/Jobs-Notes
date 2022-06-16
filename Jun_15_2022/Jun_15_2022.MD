# Notes for Jun_15_2022

This is a note or a diary for the things I research in a day, this note intended for me not to forget the knowlegde I has gain (or things I has read).

## What is Mcafee ESM Signature ID is all about

**Example Signature Id**: 47-8000253 which breakdown into these

- Befor the Dash 47 is Device Type in ESM (43 is Device Type Windows Logs, 65 is Linux Logs)
- After the dash with Windows Logs the last 4 digit is the Event Id of Windows Event Logs, the Mcafee vendor doesnt said anything about the 8000 number but as far as I know, that is the thing

The format should looks like this

>\<disd\>-\<Mcafee_Windows_Source_ID\>\<Windows_EventID (zero padded to 5 digit)\>\<Mcafee Rule Version\>

## Matplotlib Knowledge and Monthly Report

```python
plt.savefig('name.png',dpi=300,bbox_inches='tight')
```

Using **bbox_inches='tight'** to export image with the fit size
Using **dpi=300** to create img with better density of pixel 300 is suit for PDF

