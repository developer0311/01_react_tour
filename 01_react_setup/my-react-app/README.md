# **Setting Up Your Environment for React**

## **1. Online React Platform (Highly Recommended)**
For coding in React, I recommend using **CodeSandbox**, an online IDE. It’s the easiest way to dive into React without needing to configure anything locally.
Join me in learning React on CodeSandbox by clicking the link: [CodeSandbox Dashboard](https://codesandbox.io/dashboard/)

---

## **2. Local Development Environment**
If you prefer working on your machine using VSCode, you can follow these steps for setting up a local React development environment. Note that some setups may differ slightly, but you can download the lesson files to follow along easily.



- ### **Step 1: Install Node.js**
    Ensure the latest version of Node.js is installed on your system. Visit [Node.js Official Download](https://nodejs.org/en/download) and download the **LTS (Long Term Support)** version for stability.



- ### **Step 2: Install VSCode**
    Download and install the latest version of **Visual Studio Code (VSCode)** for your operating system. Get it here: [VSCode Download](https://code.visualstudio.com/download).



- ### **Step 3: Open Your Terminal**
    Use your terminal or command prompt and navigate to the folder where you want to create your React project.



- ### **Step 4: Create a Vite React App**
    Run the following command to generate a new React project using **Vite**, a fast build tool:
    ```bash
    npm create vite@latest my-react-app --template react
    ```


- ### **Step 5: Framework Selection**

    If Vite isn’t installed, the setup will prompt you to proceed. Press **Y** to continue. When asked to choose a framework, select **React** from the options.



- ### **Step 6: Choose JavaScript Variant**

    Select **JavaScript** as the variant during the setup.



- ### **Step 7: Navigate to the Project Directory**

    Move into the newly created project folder:

    ```bash
    cd my-react-app
    ```


- ### **Step 8: Install Dependencies**

    Install all required packages for your React app by running:

    ```bash
    npm install
    ```

    After installation, open the project folder in VSCode. You should see a `node_modules` directory.



- ### **Step 9: Start the Development Server**

    Run the development server using the command:

    ```bash
    npm run dev
    ```

    This command launches a local server, and any changes you make will be updated automatically.



- ### **Step 10: Open Your App in the Browser**

    Visit the local server address (usually `http://localhost:5173/`) shown in the terminal output to view your React app in action.