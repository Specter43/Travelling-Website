# Travelling-Website

Website Design Project
Friends on the way, is a website for travellers to find their ideal
fellow travellers.
This is our deployed URL: https://calm-cove-08678.herokuapp.com/

===========How to use(Roles and Features)=========================
Based on our proposal, we rearranged our functionality and features,
and there are too much code complexity in our project, so we delete the choice of
uploading a picture.

For normal user: This app's potential users are users who are passionate about
creating travel plans as well as wanting to find fellow travellers to go together.
All users have their own profile and own plans (User Profiling)
after log in(User Authentication). They can search a place for finding other user's plans,
select existing trip, choose to join the pool of users who want to take this trip, and connect users.

For admin: Our application only has one admin user in the data base.
Log in with email: admin, password: admin and you will go to the admin page.
(Authorization)
Admin can insert new recommendations, manage plans and delete existing users.


========Detailed instruction======================================
It is better for having user experience of using and grading our project
with a computer screen resolution which should be at least 1920*1080.

0. Open URL, If you are a new user, you need to sign up with valid information first.
Click "new traveller" to sign up. (You can also use Username: user; Password: user
to log in directly)

1.Follow the instruction or error message to create an account in sign up page, as required.

2.After submit, you are directed to our search page where you can search or create a plan.
With recommendations about the hottest places, you can click buttons
and move mouse to play with this page to see the view of this place.

3.Search a place you want to go, get the existing plan or create a new plan
if you are not satisfied with the result.

4.Click 鈥淐reate your plan鈥?or 鈥淪earch鈥?button on navigation bar on the top to create a plan with following information: Start Place: Los angeles, End Place: Mexico, Except Cost: 2000 dollars, Except Cost: 2000 dollars, Start Date: 2019.12.19, End Date: 2019.12.27.

5.View a plan that is created by user him/herself and
user can choose to accept or decline other users who are willing to join this plan.

6.After create an account, users can see themselves on the right of navigation bar.

7.In the profile, User can edit information and see users' plan that are created by themselves,
or other plans that they are going to.

========Overview of the routes in Express server==================

Express routes are in server.js. The file is commented properly
so you can take a look at that. Basically we have several routes for
different purposes.
One route is for User, for example: app.post('/users/signup'),app.post('/users/login'),
app.put('/editProfile'), app.get('/logout'),
The other route is for get user, user's profile, and user's plan.
Another route is for admin, for example: app.post('/admin/insertRecommendation'),
app.delete('/admin/deleteUser/:userName').
