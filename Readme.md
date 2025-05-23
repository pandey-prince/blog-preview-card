# Frontend Mentor - Blog preview card solution 

This is a solution to the [Blog preview card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/blog-preview-card-ckPaj01IcS). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Deployment](#Deployment)


## Overview 

This is a project from Frontend Mentor. In this challenges I created a blog preview card using HTML & CSS.

### The challenge

User should be able to: 
- See hover and focus states for all interactive elements on the page

### Screenshot

![](./assets/images/Screenshot%202025-05-23%20172831.png)


### Links 

- Solution URL: (https://github.com/pandey-prince/blog-preview-card)
- Live Site URL: ()

### Built with 

- Sementic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid


### What I learned 

In this project the major learning of mine is making the elements intractive.


```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="style.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Figtree:ital,wght@0,300..900;1,300..900&family=Outfit:wght@100..900&family=Roboto:ital,wght@0,100..900;1,100..900&display=swap" rel="stylesheet">
</head>
<body>
    <div class="body">
        <div class="box">
            <div class="card-img">
                <img src="/assets/images/illustration-article.svg">
            </div>
            <div class="card-details">
                <div class="learning">
                    Learning
                </div>
                <div class="published-date">
                    Published 21 Dec 2023
                </div>
                <div class="header">
                    HTML & CSS Foundation
                </div>
                <div class="para">
                    These langugage are the backbone of every website
                    ,defining struture, content, and presentation.
                </div>
                <div class="profile">
                    <div class="profile-photo">
                        <img src="/assets/images/image-avatar.webp" alt ="">
                    </div>
                    <div class="profile-name">
                        Greg Hooper
                    </div>
                </div>
            </div>
        </div>
    </div>
</body>
</html>
```

```CSS
*{
    font-family: Figtree,Arial, Helvetica, sans-serif;
    font-size :16px;
}
body{
    background-color: hsl(47, 88%, 63%);
}
.body{
    display: flex;
    align-items: center;
    justify-content: center;
    
    align-items: center;
    height:100vh;
    width:100vw;
}
.box{
    border:2px solid black;
    display:flex;
    flex-direction: column;
    justify-content: space-between;
    box-shadow:8px 8px 12px black;
    background-color: hsl(0, 0%, 100%);
    align-items: center;
    width:280px;
    border-radius:10px;
    cursor: pointer;

}
.card-img{
    margin-top:10px;
    
}


.card-img img{
    width: 250px;
    border-radius: 7px;
    
}

.card-details{
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    width: 250px;
    
    
}
.learning {
    background-color:hsl(47, 88%, 63%);
    width: 70px;
    border-radius: 4px;
    height:20px;
    text-align: center;
    font-weight: 700;
    font-size:14px;
    
    margin-bottom: 10px;

}
.learning:hover{
    box-shadow: 5px 5px 5px black;
}


.published-date{
    font-size:14px;
    
    margin-bottom: 10px;
    
}

.header{
    
    margin-bottom: 10px;
    font-weight: 800;
    transition: color 0.15s;

}
.header:hover{
    color:yellow;
}

.para{
    
    margin-bottom: 10px;
    font-weight: 400;
}

.profile{
    
    margin-bottom: 10px;
    display: flex;

}

.profile-photo img{
    height:30px;
}

.profile-name{
    font-size:14px;
    margin-left:10px;
    margin-top:6px;
    font-weight: 800;
}

.profile-name:hover{
    color:green;
}
.profile-photo img {
  transition: transform 0.3s ease;
}

.profile-photo:hover img,
.profile-photo:focus img,
.card-img:hover img
{
  transform: scale(1.05); /* slight zoom effect */
}

.profile-photo:focus {
  outline: 2px solid #facc15; /* focus ring */
  outline-offset: 4px;
}
```

### Deployment 

- For the deployment of the project I used vercel.com.
