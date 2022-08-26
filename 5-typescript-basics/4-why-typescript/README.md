### Setting up a TypeScript environment

The first step to begin coding in TypeScript is to set up a development environment. A development environment encompasses a collection of tools and procedures for developing, testing and debugging a program.
To start our development environment in Visual Studio Code, we will begin with installing **Node.js**. Node is a JavaScript runtime environment, which provides us with the ```npm``` package manager that will help us install the rest of the necessary dependencies.

To install Node.js, download the file appropriate to your Operative System from the [Node.js Website](https://nodejs.org/en/).

Once Node.js has been installed, the next step is to use the Node Package Manager to install TypeScript. This can be done *via terminal* in **Visual Studio Code**:

1. Open a new instance of VS Code.
2. Click on the Terminal tab and select *New Terminal*, **or** press *Ctrl + Shift + `*.
3. Once the terminal is open, type ```npm install -g typescript```.
4. Wait for the process to end, and TypeScript will be installed!

The last step is to create a project workspace and initialize the project. We will need to create a TypeScript file (where we will write the code to be executed).This can be done directly from Visual Studio Code:

1. Select the Explorer tab on the left pane and then select **Open Folder** or **Add a Folder** in case you have already created a folder for the project. [insert screenshot here]
2. Click on the **New File** icon and type ```helloworld.ts```.