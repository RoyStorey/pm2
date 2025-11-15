Make app that tracks what project each employee is on, and whether or not the employee is at work.

Employees:
Employee login/logout with real credential stuff
Employee Clock in/out
Employee Project
hours, minutes, seconds worked
Templated Progress Reports associated by employee

Projects:
list of projects
Project metrics (seconds worked on project)
Project milestones
Milestones per second worked?

Shop > Team > Employee

Manager Role
Employee Role

Employee View
Manager View

Database schema:
Employees
-uid
-name
-projects
-secondsWorked

Managers
-uid
-name

Projects
-uid
-name
-assignedEmployees
-secondsWorked
-pointOfContact
-deadline
-isCompleted
-dateCreated

Milestones
-uid
-associatedProject
-sequence
-associatedReport
-deadline
-isCompleted
-secondsWorked
-dateCreated

Reports
-uid
-name
-createdBy

<!-- -associatedProject -->

-associatedMilestone
-dateCreated
