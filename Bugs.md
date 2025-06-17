
## BUGS.md


### Issues Found

### Create a New Product (POST /api/products) Issue

Bug Discovery & Suggestions
Status Code Variance:
The API might return 200 OK or 201 Created for creation. This inconsistency may confuse clients. Recommend standardizing to 201 Created for resource creation.

Missing Validation:
No test checks for invalid input handling (e.g., negative price, missing required fields). Add negative tests to discover bugs related to input validation.


Duplicate Products:
No test for handling duplicate product creation. Test how the API behaves when creating a product with the same name or attributes.

Category Validation:
No test to check if the category is valid or restricted. Test with invalid categories to discover bugs.


### Check API Health (GET /health)

No JSON Response:

Issue: The endpoint returns a plain text response (healthy) instead of a JSON object (e.g., { "status": "healthy" }).

Impact: Clients expecting JSON may fail to parse the response.

Severity: Low (if clients are aware of the response format), Medium (if clients expect JSON by default).

No Additional Health Details:

Issue: The endpoint does not provide any additional health information (e.g., database status, service uptime).

Impact: Limited usefulness for monitoring and diagnostics.

Severity: Low (if only basic health is needed), Medium (if more details are required).

No Content-Type Header:

Issue: The response may not include a Content-Type: text/plain header, which could confuse clients.

Impact: Clients may misinterpret the response.

Severity: Low (if clients are tolerant), Medium (if strict parsing is required). vffffffffffffffffffffffffffffffffdcdcdcdcdcdcdcdcdcdcdcdcdcdcdcdcdcdcdcdcdcdcdcdc 
