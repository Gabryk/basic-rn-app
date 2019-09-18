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
