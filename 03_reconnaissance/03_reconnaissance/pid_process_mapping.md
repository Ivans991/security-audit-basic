# PID to Process Mapping

## Objective
The objective of this step is to associate network connections identified by netstat with their corresponding system processes.

## Method
- Network connections were identified using netstat.
- Process identifiers (PIDs) were cross-referenced using the tasklist command.

## General Findings
- Identified PIDs corresponded to known system processes and user applications.
- No unknown or suspicious process names were identified during this step.
- Observed processes are consistent with normal system behavior.

## Notes
This activity was observational only. No processes were terminated or modified.
