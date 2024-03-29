# user-api-test


# Jasmine setup with typescript
1. Initialize npm Project: 
    ```npm init```
2. Install TypeScript, Jasmine, and Jasmine types Packages: 
    ```npm i --save-dev typescript jasmine @types/jasmine```
3. Initialize Project for Typescript Usage. This will create a tsconfig.json file. 
    ```npx tsc --init```
4. Update outDir in tsconfig.json: (when compile the ts code, the complier converts ts to Js and the Js code is saved in the below directory)
    ```"outDir": "./dist", /* Specify an output folder for all emitted files. */```
5. Enable Typescript jasmine test Debugging by adding the below line in tsconfig.json:
    ```"sourceMap": true```
6. Initialize Jasmine. This creates a file at spec/support/jasmine.json
    ```npx jasmine init```
7. make the following changes in jasmine.json: To identify the Js code location genrated by the ts code compiler
    ```"spec_dir": "dist",```
8.  Add test,build and tsc in script to package.json 
   ```
    "test": "jasmine",
    "build": "tsc",
    "tsc": "tsc"
   ```
8. Create Simple TypeScript Jasmine Spec under src/my-first-test.spec.ts

9. Run build Script: 
      ```npm run tsc```
10. Run test Script: 
     ```npm test```

Reference: https://devtails.xyz/@adam/how-to-run-unit-tests-with-jasmine-and-typescript

Enable Debugging: https://code.visualstudio.com/docs/typescript/typescript-debugging
