# Intermediate Badge Submission - RAVINDU

## Task 4: Custom Workflow ✅
- Created `.github/workflows/custom.yml`
- Triggers on push to `develop` branch
- Sets up Node.js 18 and runs `npm install && npm test` in `sample-app`
- Screenshot:
  <img width="1424" height="884" alt="image" src="https://github.com/user-attachments/assets/85d13f49-7a6d-474d-a34f-4eee44fc168c" />


## Task 5: Environment Variables ✅
- Edited `.github/workflows/build-test.yml`
- Added `NODE_ENV: test` and `LOG_LEVEL: debug` at job level
- Verified values printed in "Print environment" step logs
- Screenshot:
  <img width="1426" height="892" alt="image" src="https://github.com/user-attachments/assets/afdc58a6-b83d-48d1-a28b-82eb6f5e06c5" />
  <img width="1422" height="893" alt="image" src="https://github.com/user-attachments/assets/626311d0-8c19-40fa-b6c3-20e894ef63a5" />
  <img width="1424" height="892" alt="image" src="https://github.com/user-attachments/assets/66b8c550-6e96-477a-807a-19ce3141a43c" />


## Task 6: GitHub Secrets ✅
- Created `TEST_SECRET` in repo Settings --> Secrets
- Added step to `hello-world.yml` that accesses the secret via env var
- Secret value is masked (`***`) in logs, only length is printed
- Screenshot:
  <img width="1422" height="893" alt="image" src="https://github.com/user-attachments/assets/361e57a8-2ae8-4ac7-88ee-d43a70bf8401" />


## Task 7: Matrix Testing ✅
- Modified matrix in `build-test.yml` to test Node 16.x, 18.x, 20.x
- Three parallel jobs created and ran successfully
- Screenshot:
  <img width="1424" height="894" alt="image" src="https://github.com/user-attachments/assets/f56ff761-cf3e-4a35-a19c-df461dc9fea0" />
