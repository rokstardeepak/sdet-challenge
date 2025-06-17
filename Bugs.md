
## BUGS.md


### Issues Found

1. **/health endpoint returns "healthy\n" instead of "healthy"**
   - **Description:** The `/health` endpoint returns a newline character at the end of the response.
   - **Impact:** Test assertions fail unless `.trim()` is used.
   - **Suggested Fix:** Update the endpoint to return just "healthy", or update tests to handle the newline.
