# React Web Application
Web Development is one the most common develepment area. Reactjs helps us build both web apps and native apps using the same skills. It leans upon each platform’s unique strengths to let the interfaces feel just right on every platform. React is a free and open-source front-end JavaScript library for building user interfaces based on components
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/a7/React-icon.svg/2300px-React-icon.svg.png" style="width: 300px; height: 200px;">
## Installations
To start with React application , we need to install an editor , most preferred editor is VS Code. After this , we need to install Node Js which is a powerful JavaScript runtime that allows you to build scalable and efficient web applications. NPM is the default package manager for Node.js, providing access to a vast ecosystem of libraries and tools.

## Creating first React App
Once we have installed all the required libraries , we can start by creating a suitable environment for learning ReactJs. It sets up your development environment , however it doesn't handle your backend logics or databases. It provides a basic frontend for you to get started.

 ```bash
   npx create-react-app web-tutorial
   cd web-tutorial
 ```
npx is a package runner tool.<br>
<br>

Run the following command to open the React application on browser. A new browser window pops up on port 3000 with an address : **localhost:3000**

 ```bash
   npm start
 ```
## Creating the Frontend of Website
So far so good, after this lets focus on modifying and enhancing the content of the web app. Look in the directory , you will find **src** folder, inside the folder , you have **"App.js"**, open it.

 1. **Exploring MUI:** 
 Material UI is a frontend library that helps you build components easily. It provides professionally designed components , templates and design kits to accelerate the production and enhance the UI based on our needs.Run the following command to add MUI to your project.

 ```bash
    npm install @mui/material @emotion/react @emotion/styled
 ```
 <br>

 2. **Adding JSX Elements:**
 JSX stands for Javascript XML and allows us to write HTML in React.JSX converts HTML tags into react elements.Now in 'src' folder create a file **Card.jsx** and other components like Navbar.
 <br/><br>
 Lets design the cards that displays the name and photo of people.

```bash
import * as React from 'react';
import Card from '@mui/material/Card';
import CardActions from '@mui/material/CardActions';
import CardContent from '@mui/material/CardContent';
import CardMedia from '@mui/material/CardMedia';
import Button from '@mui/material/Button';
import Typography from '@mui/material/Typography';

export default function ImgMediaCard() {
  return (
    <Card sx={{ maxWidth: 345 }}>
      <CardMedia
        component="img"
        height="140"
        image="/static/images/cards/person.jpg"
      />
      <CardContent>
        <Typography gutterBottom variant="h5" component="div">
           ARUN TIWARI
        </Typography>
        <Typography variant="body2" color="text.secondary">
           Business Development Intern
        </Typography>
      </CardContent>
      <CardActions>
        <Button size="small">View Profile</Button>
      </CardActions>
    </Card>
  );

 ```

Now , import these components in **App.js**.
 ```bash
import './App.css';
import * as React from 'react';
import Page from "./Page"
import Navbar from "./Navbar"

function App() {
  return (
    <div className="App">
      <Navbar/>
      <Page/>

    </div>
  );
}

export default App;
 ```

## Displaying Data from JS file
Create a javascript file with an array of information about people to be displayed. Now To map the data from this file into our component, we will use .map() function.


   ```bash
    Users.map(({name,title,img})=>{
      return (
        <Card sx={{ maxWidth: 345 }}>
        <CardMedia
          component="img"
          height="140"
          image={img}
        />
        <CardContent>
          <Typography gutterBottom variant="h5" component="div">
             {name}
          </Typography>
          <Typography variant="body2" color="text.secondary">
            {title}
          </Typography>
  
        </CardContent>
        <CardActions>
          <Button size="small">View Profile</Button>
        </CardActions>
      </Card>
    );
   ```

## Deploying our website

1. **Create a GitHub Repository:**
   Create a new repository on GitHub for your project.

2. **Push Your Code to GitHub:**
   Push your project to the GitHub repository.

   ```bash
   git remote add origin <your-github-repo-url>
   git branch -M main
   git push -u origin main
   ```


## Deploying on Vercel 
To deploy your React project with a Vercel for Git Integration, make sure it has been pushed to a Git repository.

Import the project into Vercel using the Import Flow. During the import, you will find all relevant options preconfigured for you with the ability to change as needed.

## Conclusion
Congratulations ! You have successfully created your first react website.
