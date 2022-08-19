
# Tips4Tips

> 

> Live demo (https://luxury-marigold-ce061c.netlify.app/). 

## Table of Contents
* [General Info]
* [Setup]
* [Room for Improvement]
* [Client - Frontend] 
* [Server - Backend] 
* [Links]
* [Acknowledgements]


## General Information
- Provide general information about your project here.
- What problem does it (intend to) solve?
- What is the purpose of your project?
- Why did you undertake it?



## Setup
What are the project requirements/dependencies? Where are they listed? A requirements.txt or a Pipfile.lock file perhaps? Where is it located?

Proceed to describe how to install / setup one's local environment / get started with the project.



## Room for Improvement/Backlog
Include areas you believe need improvement / could be improved. Also add TODOs for future development.

Room for improvement:
- Improvement to be done 1
- Improvement to be done 2

To do:
- Feature to be added 1
- Feature to be added 2


**PAGES:**

404: As an anon/user I can see a 404 page if I try to reach a page that does not exist so that I know it's my fault

Signup: As a user I can sign up in the platform so that I can start creating saving favorite markets

Login: As a user I can login to the platform so that I can see my favorite markets and follow other users

Logout: As a user I can logout from the platform so no one else can use it

Profile: As a user I can see the Markets I created and the users I follow as well as edit my profile data.

Add markets As a user I can add a market so that I can share it with the community

List markets As a user I want to all markets so that I can choose one to visit

See market details As a user I want to see the markets details so I know where I can visit it.

Review a market As a user I can click on leave a review and give my input

Search markets As a user I want to search markets by name, location or any key so that I know if it´s already in the platform

Add to favorites As a user I want to add a market to favorite so that I can save the markets that I liked the most

See my favorites As a user I want to see my favorite restaurantes so that I can see the ones I liked the most

Discover a market As a user I can click on the dicovery Button and it will show me a new Marke for me to discover.

Star a market As I user I can make my opinion about a market base on the stars a Market has. The more people has saved the market as favourite, the more stars.




<br>

# Client / Frontend

**MODELS**

USER: 

userSchema = {
  name: { type: String, required:  true }, email: { type: String, required: true }, password: { type: String, required: true }, id: { type: String },
}

POST:

postSchema = { title: String, message: String, name: String, creator: String, tags: [String], selectedFile: String, likes: { type: [String], default: [] }, comments: { type: [String], default: [] }, createdAt: { type: Date, default: new Date(),},
}


# Server / Backend

**ROUTES**

USER:

POST/signin
   - body:
     email,
     password

POST/signup
    - body:
    email, 
    password, 
    firstName, 
    lastName

POSTS:

GET/creator
     query:
     name,



GET/search
     query:
     searchQuery,
     tags,

  


GET/posts
    query:
    page,

 
GET/posts/:id

POST/auth //createPost 

PATCH/:id //updatePost

DELETE/:id //deletePost

PATCH/:id/ //likePost

POST/:id  //commentPost

## Links

### Trello

(https://trello.com/b/MdJEGVrC/project-module-3) 


### Git


[Client repository Link](https://github.com/Gabriel-PF/Tips4Tips-client)

[Server repository Link](https://github.com/Gabriel-PF/Tips4Tips-server)

[Deployed App Link](https://luxury-marigold-ce061c.netlify.app/posts)

### Slides

The url to your presentation slides

[Slides Link](https://docs.google.com/presentation/d/1zndKZ8DC-_i391alptPKsAKanCSXTrLVL39L3xtEjz8/edit?usp=sharing)

## Acknowledgements
Give credit here.
- This project was inspired by...
- This project was based on [this tutorial](https://www.example.com).
- Many thanks to...


