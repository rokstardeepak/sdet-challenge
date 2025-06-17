# SDET Challenge API Test Suite

This repository contains the test suite for the SDET Challenge API.

## How to Run the Tests

1. **Install Postman** (https://www.postman.com/downloads/)
2. **Import the collection:**
   - Open Postman.
   - Click **Import**.
   - Upload `sdet-challenge-api.postman_collection.json`.
3. **Set environment variables** (if needed):
   - Import your environment file.
   - Set `baseUrl` and `token` as required.
4. **Run the tests:**
   - Open the collection.
   - Click **Run** to execute all tests.

## Automated Testing

You can also run the tests from the command line using [Newman](https://github.com/postmanlabs/newman):

npm install -g newman
newman run sdet-challenge-api.postman_collection.json

## Bugs and Issues

See [BUGS.md](BUGS.md) for a list of issues found during testing.
