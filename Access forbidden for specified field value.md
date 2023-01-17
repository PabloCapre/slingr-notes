# Access forbidden for specified field value

This issue was originated when I tryed to create a new TT record using a Frontend user.

When I check the field permission in the record entity was all right. The group user was able to Read/Writte.

That field was a related one, pointing to another entity. So the issue was that the group user haven't access to the related entity.

To fix it, I gave access permission to that group user to the related entity.

## Solved.