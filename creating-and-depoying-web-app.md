# Creating and Deploying a Simple Web Application: A Step-by-Step Guide

## Introduction

Building and deploying a simple web application is an exciting way to learn the basics of web development. This guide provides a step-by-step process for creating a minimal web application and deploying it to a hosting service. We'll use HTML, CSS, and JavaScript for the frontend, and we'll deploy our application on a cloud platform.

## Prerequisites

Before you start, ensure you have the following:

- A text editor (e.g., Visual Studio Code, Sublime Text)
- Basic knowledge of HTML, CSS, and JavaScript
- Node.js and npm installed on your machine

## Step 1: Set Up Your Project

1. **Create a Project Directory:**
   Open your terminal and create a new directory for your project.

   ```bash
   mkdir simple-web-app
   cd simple-web-app
   ```

2. **Initialize npm:**
   Initialize npm in your project directory.

   ```bash
   npm init -y
   ```

   This will create a `package.json` file.

## Step 2: Create the Frontend

1. **Create HTML File:**
   Create an `index.html` file in your project directory and add basic HTML structure.

   ```html
   <!DOCTYPE html>
   <html lang="en">
   <head>
       <meta charset="UTF-8">
       <meta name="viewport" content="width=device-width, initial-scale=1.0">
       <title>Simple Web App</title>
       <link rel="stylesheet" href="styles.css">
   </head>
   <body>
       <h1>Hello, World!</h1>
       <script src="app.js"></script>
   </body>
   </html>
   ```

2. **Create CSS File:**
   Create a `styles.css` file in the same directory.

   ```css
   body {
       font-family: Arial, sans-serif;
       text-align: center;
   }

   h1 {
       color: #3498db;
   }
   ```

3. **Create JavaScript File:**
   Create an `app.js` file in the same directory.

   ```javascript
   console.log('Hello from app.js!');
   ```

## Step 3: Test Locally

1. **Open in Browser:**
   Open your `index.html` file in a web browser to ensure everything is rendering correctly.

## Step 4: Deploy to GitHub

1. **Create a GitHub Repository:**
   Create a new repository on GitHub for your project.

2. **Push Your Code to GitHub:**
   Push your project to the GitHub repository.

   ```bash
   git remote add origin <your-github-repo-url>
   git branch -M main
   git push -u origin main
   ```

## Step 5: Deploy to a Cloud Platform

1. **Choose a Cloud Platform:**
   Choose a cloud platform for hosting your web application. Options include Heroku, Netlify, or Vercel. We'll be using Netlify for deployment in this tutorial.

2. **Create an Account:**
   Create an account on Netlify. You can signin using any of the mentioned methods.
   <img src="https://github.com/MonalikaPatnaik/Technical_Writing/assets/99353300/3d199ea1-13aa-4fb0-99fb-3b584fb63e1d" style="width: 400px; height: 400px;">


4. **Initiating a New Site on Netlify Dashboard:**
   Next, You will be redirected to the Netlify dashboard. Then, click on "New site from Git".
   <img src="https://github.com/MonalikaPatnaik/Technical_Writing/assets/99353300/5ee32f37-3bfa-424e-aaaa-5b10491124e2" style="width: 600px; height: 300px;">
  

6. Then, Choose GitHub.<br>
   <img src="https://github.com/MonalikaPatnaik/Technical_Writing/assets/99353300/975bc0b8-c668-45e8-a343-6a94c3c65330" style="width: 600px; height: 300px;">
   
8. Next, choose the repository that you want to deploy and click on the deploy site button.
   <img src="https://github.com/MonalikaPatnaik/Technical_Writing/assets/99353300/3d5be1b2-5edd-406f-bc5f-7371d4752866" style="width: 600px; height: 400px;">
  
Next, wait for a few seconds and you will see that it shows you a message with the link to your website.


## Conclusion

Congratulations! You've successfully created a simple web application and deployed it to a hosting service.
