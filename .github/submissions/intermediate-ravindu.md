# Intermediate Badge Submission — RAVINDU

## Task 4: Custom Workflow ✅
- Created `.github/workflows/custom.yml`
- Triggers on push to `develop` branch
- Sets up Node.js 18 and runs `npm install && npm test` in `sample-app`
- [Screenshot: Actions tab showing Custom Workflow run]

## Task 5: Environment Variables ✅
- Edited `.github/workflows/build-test.yml`
- Added `NODE_ENV: test` and `LOG_LEVEL: debug` at job level
- Verified values printed in "Print environment" step logs
- [Screenshot: Logs showing environment values]

## Task 6: GitHub Secrets ✅
- Created `TEST_SECRET` in repo Settings --> Secrets
- Added step to `hello-world.yml` that accesses the secret via env var
- Secret value is masked (`***`) in logs, only length is printed
- [Screenshot: Log showing "Secret length: 15" with masked value]

## Task 7: Matrix Testing ✅
- Modified matrix in `build-test.yml` to test Node 16.x, 18.x, 20.x
- Three parallel jobs created and ran successfully
- [Screenshot: Actions tab showing 3 parallel matrix jobs]