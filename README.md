
### Tips4Tips ###

> A full stack MERN application with all CRUD operations capabilities delivering a social media platform where users can share their little secrets and tips in their favorite places. 

> Live demo (https://luxury-marigold-ce061c.netlify.app/). 

## Table of Contents
* [General Info]
* [Room for Improvement - backlog]
* [Pages]
* [Client - Frontend - Models] 
* [Server - Backend - Routes] 
* [Links]
* [Acknowledgements - Inspiration]


## General Information

With the massification of the tourism and the rise of social media, the tendency nowadays is for people simply trying to mimic influencers when traveling, going to overrated places, basically "believing the hype", since several of those places and attractions can be paid promotion or product placement, we come up with this idea to provide a platform for more "obscure" travel tips where you can find not so obvious advices and "workarounds" for popular destinations, if your tip is indeed a good one, the user can actually earn some tips. 
Other functionality to be implemented is the possibility to create closed networks so friends and family can share their expediencies in a more private setting. 


## Room for Improvement/Backlog
Include areas you believe need improvement / could be improved. Also add TODOs for future development.

Room for improvement:
- Fix:
     .bugs
     .tags function when creating posts and searching.
     
- More models and functionalities, user settings, and personalization. 

To do:
- Implementing a "tip jar" functionality with PayPal integration
- Implement a way so that users can create closed groups or networks in order to share their tips in a private enviroment. 
- Possibility to edit and delete comments

**PAGES:**

404: As an anon/user I can see a 404 page if I try to reach a page that does not exist so that I know it's my fault

List of all posts created by the users of the platform even if not logged in. 

Signup: Users can sign up. 

Login: Users can login and create their own posts. 

Logout: Users can logout and continuing navigating through the posts and even posts "anonymous" comments. 
 
See posts details more in depth information regarding the post and also the comments attached. 

Search for specific post, user is able to search for a specific tittle or keyword. 

Edit a post, user creator of the post is able to edit all tittle, description and picture of the post. 

Comment in a post, user I can see the post details and leave a feedback.

Like a post, user is able to like the posts based on their content. 


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

### Links

## Trello

(https://trello.com/b/MdJEGVrC/project-module-3) 


## Git


[Client repository Link](https://github.com/Gabriel-PF/Tips4Tips-client)

[Server repository Link](https://github.com/Gabriel-PF/Tips4Tips-server)

[Deployed App Link](https://luxury-marigold-ce061c.netlify.app/posts)

## Slides

The url to your presentation slides

[Slides Link] - (https://docs.google.com/presentation/d/1rC83HJCVXhQzczrAxFxwXivNT1WlTG1QA560ICoqTw4/edit?usp=sharing)

## Acknowledgements

- This project was inspired by:

 (https://www.youtube.com/watch?v=zaWtIkJgah4&ab_channel=JohnAhn)
 (https://www.youtube.com/watch?v=TFGEq5OZgaA&ab_channel=IndianCoders)

- Many thanks to the teacher and colleagues