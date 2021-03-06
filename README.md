# Color me

This project is showing how you can use Office.js and Angular 4 to build an Excel add-in.

## How to run

1. To run the add-in, you need side-load the add-in within the Excel application. The section below describes the way of side-loading of manifest file in different platforms.

    - On Windows, follow [this tutorial](https://dev.office.com/docs/add-ins/testing/create-a-network-shared-folder-catalog-for-task-pane-and-content-add-ins).

    - On macOS, move the manifest file `office-add-in-angular-manifest.xml` to the folder `/Users/{username}/Library/Containers/com.microsoft.Excel/Data/Documents/wef` (if not exist, create one)

    - For Excel Online, use the upload my add-in button from the add-in command dialog to upload the manifest file. 

2. Run `ng serve` or `npm start` in the terminal for a dev server.

3. Open Excel and click the Add-in to load.

<img width="1156" alt="angular" src="https://user-images.githubusercontent.com/3375461/28433959-85c503a0-6d42-11e7-8766-98e953179e2d.png">

## How to create a new project by yourself

1. Generate the Angular project using [Angular CLI](https://github.com/angular/angular-cli).

2. Generate the manifest file using [YO Office](https://github.com/OfficeDev/generator-office). When you generate, choose only generating the manifest file.
Then replace all the ports in the generated manifest file from `3000` to `4200`.

## Learn more 

To learn more about JavaScript API for Office (Office.js), please check [here](https://dev.office.com/reference/add-ins/javascript-api-for-office).
