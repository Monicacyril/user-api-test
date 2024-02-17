# user-api-test


# Jasmine setup with typescript
1. Initialize npm Project: 
    ```npm init```
2. Install TypeScript, Jasmine, and Jasmine types Packages: 
    ```npm i --save-dev typescript jasmine @types/jasmine```
3. Initialize Project for Typescript Usage. This will create a tsconfig.json file. 
    ```npx tsc --init```
4. Update outDir in tsconfig.json: 
    ```"outDir": "./dist", /* Specify an output folder for all emitted files. */```
5. Add test,build and tsc in script to package.json 
   ```"test": "jasmine",
    "build": "tsc",
    "tsc": "tsc"```
6. Create Simple TypeScript Jasmine Spec under src/my-first-test.spec.ts

7. Run build Script: 
      ```npm run tsc```
8. Run test Script: 
     ```npm test```
    
