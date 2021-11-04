# IronGram

Frontend:

HomePage /
AboutPage /about
LogIn /login
Signup /signup
Profile Page (public) /:user
Profile Settings (private) /settings
Feed Page (logged in) /feed
Post Page (individual, public) /post/:postId

Backend:
/auth/login POST
/auth/signup POST
/auth/logout DELETE
/auth/delete-account
/profile/:userId GET
/profile/:userId/edit PUT
/auth/me GET (get loggedin user data)
/feed GET
/post/:postId GET
/post/add POST
/post/edit POST
/post/delete DELETE
/post/like PUT
/user/follow PUT

IF WE HAVE TIME:
FOLLOW USERS


Models:
User
username: string
password: string
following: User[]

Post
content: string
image: string
likes: User[]
owner: User

Session
userId: ObjectId(User)