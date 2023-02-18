# Date common format in Slingr

## Date format MM-dd-YYYY and 00:00hs Slingr Platform

Create a new date object:`var today = new Date()`

Set hours to 00:00: `today.setHours(0,0,0,0);`

And finally the format: `sys.utils.time.format(today, 'MM-dd-yyyy')`