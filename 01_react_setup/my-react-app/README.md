# **Local Development Setup**

## **Step 1:**

Make sure you have the latest version of Node installed. If not head over to https://nodejs.org/en/download to download the LTS (Long Term Support) version of Node.

## **Step 2:**

Make sure you have the latest version of VSCode installed. If not, head over to https://code.visualstudio.com/download to download the version for your platform.

## **Step 3:**

Open a Terminal or command prompt and navigate to the directory where you want to create your React project.

## **Step 4:**

Create a Vite app by running the following command in your Terminal or Command Prompt:

```bash
npm create vite@latest my-react-app --template react
```

## **Step 5:**

The first time, you won't have Vite installed. Type y to proceed. Then you'll be asked to select a framework. Use your down arrow to select React.

## **Step 6:**

You'll be asked to select a variant, select Javascript.

## **Step 7:**

Change directory to the new app that you built.

```bash
cd my-react-app
```

## **Step 8:**

Install dependencies:

```bash
npm install
```

When npm has installed all the necessary packages, open your project folder in VS Code. You should see a node modules folder.

## **Step 9:**

Start the development server:

```bash
npm run dev
```

Vite will compile your code every time your change anything and you can see the location of your development server in the output.

## **Step 10:**

Open the app in your browser by heading over to the local address shown. It's usually at http://localhost:5173/
