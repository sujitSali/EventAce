# EventAce

Problem
--------

Using Win32::Eventlog module.
-------------------------------

What happens for each eventlog we read, it generates a Microsoft audit event in the security eventlog. Unfortunately, when you read thousands of logs, you generate thousands of audit events. This is a problem.

However using POWERSHELL generates 1 audit event for the entire reading of the eventlogs.

However, POWERSHELL is sllooooww. in fact 2 to 3 times slower than the current method and it doesn't work on both Windows and Linux.

We need to create a utility or library that will behave like powershell to the audit system.
-------------------------------------------------------------------------------------------

