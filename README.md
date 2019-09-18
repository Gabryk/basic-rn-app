# basic-rn-app
Basic App with React Native, CircleCI 


## Setup Google credentials for API Access
Generate the needed .json file: https://docs.fastlane.tools/getting-started/android/setup/#collect-your-google-credentials

### For CI
For CI define de ENV var GO_SERVICE_ACCOUNT as json.

### For local dev
Place the file into `/android/service_account.json` folder. 

## Generating an upload keys for Android

### For CI
Define ENV var GO_UPLOAD_KEYSTORE as base64 string.

### For local dev
Make sure you place the keystore in `android/app/upload.keystore`

Also make sure to define cretificates password as ENV vars:

### Keys credentials
KEY_ALIAS=androiduploadkey
KEY_PASSWORD=android
STORE_PASSWORD=android


## Deploying an Alpa release
Create a git Tag as `v.`.
E.g. `v.0.1`
This will tryger the CI Job to deploy the an Alpa release.

## Deploy a Beta release
To release the Beta you only need to approve the Hold Job in Circle CI. So just navigate to Circleci platform, find the build register and approve it.

**MoreInfo:** https://circleci.com/docs/2.0/workflows/