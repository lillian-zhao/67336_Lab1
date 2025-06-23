# Lab 1: JavaScript Foundations

It is **crucial** that you read the following instructions before working on anything in this project.
Throughout this lab, make sure to commit regularly and push your changes to GitHub.

***Have fun learning Javascript!***

---


## Step 1: Check for Node.js and VSCode

Make sure Node is installed by going to your terminal and typing the following command:

```bash
node -v
```

If not, download it from [https://nodejs.org](https://nodejs.org). Also install [VSCode](https://code.visualstudio.com/) if you haven’t already.

## Step 2: Clone the Starter Repository

1. Create a folder on your computer for 67-336. Open Terminal at this folder by CD-ing into it. Please refer to this documentation for help on how to do this: [Basic Git Commits](https://gist.github.com/bradtraversy/cc180de0edee05075a6139e42d5f28ce). 

2. Clone the repo using this command:

```bash 
git clone https://github.com/CMU-67336-Data-Visualization/Lab01_JavaScriptFoundations.git
cd Lab01_JavaScriptFoundations
```

## Step 3: Create Your Own Private GitHub Repo

1. Go to [GitHub](https://github.com) and create a new **private** repository named:

```
lab-1-67336
```

2. Go to **Settings > Collaborators** and add:

- `shihongh`
- `wenchaohu1`
- `lexik04`

You **must** do this so we can grade your lab.

## Step 4: Connect the Starter Repo to Your New GitHub Repo

### 1. Check the Current Remote

```bash
git remote -v
```

You should see:

```
origin  https://github.com/CMU-67336-Data-Visualization/Lab01_JavaScriptFoundations.git (fetch)
origin  https://github.com/CMU-67336-Data-Visualization/Lab01_JavaScriptFoundations.git (push)
```

### 2. Remove the Existing Remote

```bash
git remote remove origin
```

Verify it was removed:

```bash
git remote -v
```

_No output means success._

### 3. Add Your New Remote

```bash
git remote add origin https://github.com/YOUR-USERNAME/lab-1-67336.git
```

Replace `YOUR-USERNAME` with your GitHub username.  
Verify:

```bash
git remote -v
```

You should now see your personal repo. 

Initiate with the following command to initialize a package.json for the lab:

```bash
npm init -y
```

This will create a package.json file. Open package.json and replace the "scripts" section with:

```bash
"scripts": {
  "start": "node index.js",
  "test": "echo \"Error: no test specified\" && exit 1"
}
```

### 4. Push to Your Repository

```bash
git add .
git commit -m "Initial commit from starter repo and created package.json"
git push --set-upstream origin main
```
Go to Github, please make sure the files are populated into your repository. If not, please stop, and ask for help. 


## Step 5: Use a Development Branch

For best coding practices, you should **not** be working on the main branch. To keep your `main` branch clean:

1. Create a new branch.
```bash
git checkout -b lab-dev
```

2. Make any changes you want to any file, then:

```bash
git add .
git commit -m "Made updates"
git push -u origin lab-dev
```

3. After you make sure the code is correct, you can merge onto main branch: 

```bash
git checkout main
git merge lab-dev
git push
``` 

## Step 6: Run the Starter Code

Inside the project directory, install Node dependencies (if any) and run the code.

```bash
npm install
npm start
```

You should see:

```
Hello, World!
```

## Step 7: Follow the comments and complete the index.js and index.html files. 

## Step 8: Deployment on Vercel

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

## Step 9: Submitting on Canvas

Submit the following:

- Your **GitHub repo link**
- Your **Vercel live site link**

⚠️ Don’t forget to add `shihongh`, `wenchaoh`, `lexik04` as collaborators on GitHub so we can grade your lab!

-- 

That’s it! You’ve cloned a project, set up Git, deployed on Vercel, and written some JavaScript!
