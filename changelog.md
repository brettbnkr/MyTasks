# Change Log for MyTasks

## v1.8.0

+ Fixed Task Category bug (Issue #26) Thank you @shaneis
+ revised Pester test for category fix
+ Updated `README.md`

## v1.7.0

+ file cleanup for PowerShell Gallery
+ moved aliases to function definitions
+ Added auto completer for `Get-MyTask`, `Set-MyTask`, `Complete-MyTask`, `Remove-MyTask` (Issue #32)
+ Updated `Get-MyTask` to support multiple ID numbers (Issue #31)
+ help documentation update
+ general code cleanup

## v1.6.0

+ Fixed bug saving XML to non-filesystem paths (Issue #28)
+ Update `Set-MyTaskPath` to support -Passthru (Issue #25)
+ Updated `Get-EmailReminder` to include additional details (Issue #18)
+ Fixed CSS bug in email scriptblock
+ Updated `Enable-EmailReminder` to let user specify number of days (Issue #29)
+ Updated `Enable-EmailReminder` to let user specify alternate path (Issue #30)
+ updated Pester tests
+ updated documentation

## v1.5.1

+ fixed bug with MyTaskCategory (Issue #27)

## v1.5.0

+ Added a patch to store date in an ISO friendly format. (Issue #23 and Issue #22)
+ Added a new function, `Set-MyTaskPath` to allow you to update the task folder (Issue #20)
+ Updated documentation

## v1.4.0

+ Added support for PowerShell scheduled job to email upcoming tasks (Issue #17)
+ Scheduled reminders will be a Windows only feature.
+ Added timestamp to verbose messages

## v1.3.1

+ fixed bug with Show-Task when no entries are found (Issue #16)
+ Updated README

## v1.3.0

+ Updated README
+ Added 'task' as an alias for New-MyTask
+ Added CompletedDate parameter to Complete-MyTask (Issue #13)
+ Added option to complete a task by ID (Issue #11)
+ Changed default for `Get-MyTask` and `Show-MyTask` to display tasks due in next 30 days. (Issue #12)
+ fixed bug in `Show-MyTask` where completed tasks were displaying in red
+ Made parameters for `New-MyTask` more positional (Issue #14)
+ Updated help documentation

## v1.2.0

+ Modified files to support PowerShell Core
+ Update help documentation
+ Updated `README.md`
+ Updated manifest

## v1.1.0

+ Updated verbose messages
+ moved class definition to functions script
+ revised Pester tests

## v1.0.4

+ explicitly added UTF8 encoding when reading and writing XML content.
+ explicitly added Unicode encoding when reading and writing task category file. (Issue #4)
+ Modified Show-MyTask to format as a table with autosize and string streaming.
+ Updated manifest

## v1.0.3

+ modified code when creating a new XML file to declare
+ encoding as UTF-8.
+ Modified `Get-MyTask` to display a warning when trying to display tasks
+ when none have been defined yet.
+ Modified `Show-MyTask` to work under the Windows 10
+ PowerShell ISE (Issue #2)
+ Modified `Remove-MyTask` to accept MyTask as an input object (Issue #3)
+ Help files are NOT updated yet to reflect these changes.
+ Updated `README.md`

## v1.0.2

+ modified `New-MyTask` so that passthru displays
+ the correct ID. (Issue #1)

## v1.0.1

+ Added Pester tests
+ fixed a bug with exported variables

## v1.0.0

+ added license file
+ bumped version number
+ initial release

## v0.0.16

+ Added help documentation
+ Revised `Save-MyTask` to save a single task.
+ Revised `Complete-MyTask` to archive a single task.
+ Modified `Get-MyTask` to allow wildcards for -Name.

## v0.0.15

+ fixed a regular expression bug in `Show-MyTask` that wasn't properly capturing completed tasks.
+ Modified `Show-MyTask` to display completed tasks in green.
+ Added command `Save-MyTasks` move completed tasks to an archive file.
+ Modified `Complete-MyTask` with an option to archive.

## v0.0.14

+ modified `Set-MyTask` to use task ID
+ fixed a regular expression bug in `Show-MyTask`

## v0.0.13

+ Renamed Backup-MyTask to `Backup-MyTaskFile`
+ Modified module to export `Backup-MyTaskFile`
+ Modified `Remove-MyTask` to use `Backup-MyTaskFile`

## v0.0.12

+ Added `Backup-MyTask`
+ modified `mytasks.format.ps1xml` file to display DueDate without time when using tables. Format-List will show full DueDate value.
+ Added parameter to `New-MyTask` to allow specifying a number of days instead of an actual date.

## v0.0.11

+ Modified `Get-MyTask` to not include completed tasks when filtering by DaysDue or Category.
+ Added `Get-MyTaskCategory`
+ Added `Add-MyTaskCategory`
+ Added `Remove-MyTaskCategory`

## v0.0.10

+ Modified `Get-MyTask` to support filtering by number of days due
+ Modified Refresh() method to not mark a task as overdue if it is completed.
+ Modified `Show-MyTask` to not flag Completed tasks
+ Modified `Get-MyTask` to automatically sort on DueDate

## v0.0.9

+ Added comment based help
+ Changed TaskCategory to a string and used dynamic parameters in functions.
+ Modified `Show-MyTask` to support -Category
+ Adjusted settings in format.ps1xml file

## v0.0.8

+ updated `MyTasks.format.ps1xml` file with new views
+ updated `MyTasks.format.ps1xml` to format DueDate
+ added verbose output to commands
+ Modified `Get-MyTask` to support filtering by Category
+ Modified `Show-MyTask` to display in yellow if due date is 24 hours or less

## v0.0.7

+ added `MyTasks.format.ps1xml`
+ fixed a bug in `Set-MyTask` when there was an empty value
+ updated module files

## v0.0.6

+ added `Complete-MyTask` function
+ fixed a bug in `New-MyTask` when XML file exists but has no objects
+ Added -WhatIf to `New-MyTask`

## v0.0.5

+ Added `Set-MyTask` function
+ Modified `Get-MyTask` to take name as a positional parameter
+ added command aliases
+ Updated module files

## v0.0.4

+ Added `Remove-MyTask` function

## v0.0.3

+ Added `Show-MyTask` function

## v0.0.2

+ Import tasks from XML file
+ Get tasks from XML file with options
+ separated functions into their own file
+ modified class so that OverDue and ID values are calculated at runtime.
+ Added changelog

## v0.0.1

+ added core module files
