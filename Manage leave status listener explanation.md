## Manage leaves status

Type `Data` for `Management > Leaves`:
* On record created (no condition)
* On record changed (no condition)
If a Leave was **created** with `approved` status, it'll send a
notification to the leave's associate.
If a Leave was **changed** and has now status `inProgress`, it'll
verify:
* if it's a *paid vacation*, will update user's vacation days and add
the leave.
* if it's a *non-paid leave*, it'll find the user's Work
Agreement and will calculate the unpaid leave compensation.
If it's none of the above, it'll verify if the new status is `stopped`
and will look for holidays, it'll verify if it has been discounted (compensation) in case of *non-paid leave*, or if it is a *paid vacation*, it'll verify if the days have been substracted.
If the new status is `cancelled`, it'll send a notification.