# Welcome to the VS Code Hydrate Extension

This extension will allow users to select a Kubernetes cluster to run Hydrate
on. This quickstart guide will be continuously updated as features are added.
Currently, the extension builds upon the existing
[`VSCode Kubernetes Extension`](https://github.com/Azure/vscode-kubernetes-tools).
Upon right-clicking a cluster, an option to "Hydrate Cluster" is shown.
Hydrating the selected cluster will generate a `component.yaml` file in the same
directory as the user's Hydrate clone.

## What's in the folder

-   This folder contains all of the files necessary for your extension.
-   `package.json` - this is the manifest file in which you declare your
    extension and command.
    -   The sample plugin registers a command and defines its title and command
        name. With this information VS Code can show the command in the command
        palette. It doesn’t yet need to load the plugin.
-   `src/extension.ts` - this is the main file where you will provide the
    implementation of your command.
    -   The file exports one function, `activate`, which is called the very
        first time your extension is activated (in this case by executing the
        command). Inside the `activate` function we call `registerCommand`.
    -   We pass the function containing the implementation of the command as the
        second parameter to `registerCommand`.

## Get up and running

-   Press `F5` to open a new window with your extension loaded.
-   Click the Kubernetes icon in the sidebar to open the Kubernetes extension.
    Once the clusters load, right-clicking a cluster will display an option to
    `Hydrate Cluster`.
-   Clicking `Hydrate Cluster` will generate a `component.yaml` file in the same
    directory as the Hydrate clone. Check the debug console for output from the
    `Hydrate` module and for any error messages.
-   Set breakpoints in your code inside `src/extension.ts` to debug your
    extension.
-   Find output from your extension in the debug console.

## Make changes

-   You can relaunch the extension from the debug toolbar after changing code in
    `src/extension.ts`.
-   You can also reload (`Ctrl+R` or `Cmd+R` on Mac) the VS Code window with
    your extension to load your changes.

## Explore the API

-   You can open the full set of our API when you open the file
    `node_modules/vscode/vscode.d.ts`.

## Run tests

-   Open the debug viewlet (`Ctrl+Shift+D` or `Cmd+Shift+D` on Mac) and from the
    launch configuration dropdown pick `Extension Tests`.
-   Press `F5` to run the tests in a new window with your extension loaded.
-   See the output of the test result in the debug console.
-   Make changes to `test/extension.test.ts` or create new test files inside the
    `test` folder.
    -   By convention, the test runner will only consider files matching the
        name pattern `**.test.ts`.
    -   You can create folders inside the `test` folder to structure your tests
        any way you want.

## Go further

-   Reduce the extension size and improve the startup time by
    [`bundling your extension`](https://code.visualstudio.com/api/working-with-extensions/testing-extension).
-   [`Publish your extension`](https://code.visualstudio.com/api/working-with-extensions/publishing-extension)
    on the VSCode extension marketplace.
-   Automate builds by setting up
    [`Continuous Integration`](https://code.visualstudio.com/api/working-with-extensions/continuous-integration).
