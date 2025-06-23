# Lab 1: JavaScript Foundations

<br>
It is ***crucial*** that you read the following instructions before working on anything in this project.
Throughout this lab, make sure to commit regularly and push your changes to GitHub.
<br> 

***Have fun learning Javascript!***
## Step 1: Check for Node.js and VSCode

Make sure Node is installed by going to your terminal and typing the following command:

```bash
node -v
```

If not, download it from [https://nodejs.org](https://nodejs.org).  
Also install [VSCode](https://code.visualstudio.com/) if you haven’t already.

## Step 2: Create Your GitHub Repository

1. Go to [GitHub](https://github.com) and create a new **private** repository named:

```
lab-1-67336
```

2. Go to **Settings > Collaborators** and add:

- `shihongh`
- `wenchaohu1`
- `lexik04`

  [You must do this step for us to be able to grade your submission!]

## Step 3: Set Up Local Folder

Create a folder on your computer to store all your future labs for 67-336. Create a sub-folder for lab 01. 

Open a Terminal window at this folder by cd-ing into it (refer to this: https://gist.github.com/bradtraversy/cc180de0edee05075a6139e42d5f28ce) and run the following command to initialize the local Git repository:

```bash
git init
```

Then link to your GitHub repo:

```bash
git remote add origin https://github.com/YOUR-USERNAME/lab-1-67336.git
```
(Replace `YOUR-USERNAME` with your actual GitHub username.)

## Step 4: Initialize the Project
Initiate with the following command to initialize a package.json for the lab:

```bash
npm init -y
```
This will create a `package.json` file.  
Open `package.json` and replace the scripts section with:

```json
"scripts": {
  "start": "node index.js",
  "test": "echo \"Error: no test specified\" && exit 1"
}
```

## Step 5: Write Hello World

Create an `index.js` file:

```bash
touch index.js
```

Add this inside `index.js` add the following code:

```javascript
console.log('Hello, World!');
```

Now test that everything works by running the start script we added earlier to run the index.js file in the terminal:

```bash
npm start
```

You should see:

```
Hello, World!
```

Congrats! You just wrote your first "Hello World" program in Javascript!

Follow the next steps to get the starter files for the coding portion of the lab.

## Step 6: Get the Starter Code

Clone the starter repo into a **new folder**:

```bash
git clone https://github.com/CMU-67336-Data-Visualization/Lab01_JavaScriptFoundations.git
```

Copy `index.js` and `index.html` from that repo into your current lab folder, replacing your current `index.js`.

---

## Step 7: Deployment on Vercel

We’ll use [Vercel](https://vercel.com) to deploy your JavaScript project.

### 1. Create a Vercel Account

Go to [https://vercel.com](https://vercel.com) and sign up with your **GitHub account**.

### 2. Import Your Project from GitHub

1. On the Vercel dashboard, click **“Add New Project”**.
2. Select your `lab-1-67336` repo.
3. For **Framework Preset**, choose **Other** (since this is a basic HTML + JS project).
4. Make sure the following settings are correct:
   - **Root Directory**: `./` (or leave blank)
   - **Build Command**: _Leave blank_
   - **Output Directory**: `./` or _Leave blank_

Then click **Deploy**.

### 3. Get Your Live URL

After deployment finishes, you’ll get a live preview URL like:

```
https://lab-1-67336-yourname.vercel.app/
```

## Step 8: Submitting on Canvas

Submit a your **Vercel URL** in your Canvas submission and your GitHub repo link!

⚠️ Don’t forget to add `shihongh`, `wenchaoh`, `lexik04` as collaborators on GitHub so we can grade your lab!
