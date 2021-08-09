
# **project--3

## ONLYPAGES:


## OUR PURPOSE:



# **TRELLOBOARD:**

<img width="1440" alt="Screen Shot 2021-08-08 at 8 44 21 PM" src="https://user-images.githubusercontent.com/86076993/128650989-c5288a2d-1af8-4a61-b83a-23e345c9976b.png">

https://trello.com/b/psQLIPk4/project-3

ERD:



# **SCREENSHOTS:**




# **SAMPLECODE:**

SAMPLE
````

// post s.1.6 import router from express 
import { Router } from 'express'

//post s.1.7 import post controller
import * as postsCtrl from "../controller/posts.js"


// define s.1.8
const router = Router()

export{
    router 
}

// post s.1.9 make get request for posts
router.get('/', isLoggedIn, postsCtrl.index)

// post s.2.2 make a post request for post
router.post('/', isLoggedIn, postsCtrl.create)

// post s.3.2 make a get/:id request for post
router.get('/:id', isLoggedIn, postsCtrl.show) 

// post s.4.2 make a get/:id request for post
router.delete('/:id', isLoggedIn, postsCtrl.delete)

// post s.5.2 make a get/:id request for edit
router.get('/:id/edit', isLoggedIn, postsCtrl.edit)

// post s.6.2 make a put/:id request for put
router.put('/:id', postsCtrl.update)

// post s.7.2 make a post/:id request for post
router.post('/:id', isLoggedIn, postsCtrl.reply)

function isLoggedIn(req, res, next) {
    if (req.isAuthenticated()) return next();
    res.redirect("/auth/google");
  }


````


# **TECH USED**

POSTMAN:

API:

BOOTSCRAP:

GITHUB:

SOCKET IO:

REACT: 

GOOGLE OAUTH:

MONGOOSE:

MONGODB:


# **ICE BOX**


- [ ] Author video sessions

- [ ] event

MORE

# **RESOURCES**


# **CREDIT**

