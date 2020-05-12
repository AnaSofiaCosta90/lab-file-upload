![logo_ironhack_blue 7](https://user-images.githubusercontent.com/23629340/40541063-a07a0a8a-601a-11e8-91b5-2f13e4e6b441.png)

# Express File Upload

## Requirements

- [Fork this repo](https://guides.github.com/activities/forking/)
- Clone this repo into your `~/code/labs`

## Submission

Upon completion, run the following commands

```
$ git add .
$ git commit -m "done"
$ git push origin master
```

Navigate to your repo and create a Pull Request -from your master branch to the original repository master branch.

In the Pull request name, add your name and last names separated by a dash "-".

## Deliverables

Complete all of the non-bonus iterations. No styling is required, but is suggested as bonus.

## Instructions

## Introduction

<img src="https://s3-eu-west-1.amazonaws.com/ih-materials/uploads/upload_c0b2a46765e63ac8ac589835f7bb92ea.png" width="500px">

[Tumblr](tumblr.com) is an ultra popular microblogging website.

### Iteration 1 | User Profile Pictures

We've already provided a User model and the authentication logic. Unfortunately, the user doesn't have a profile picture.

Fix the User Registration so that it allows the user to upload a file as their profile image.

### Iteration 2 | Posts

In this iteration, create the bread and butter of Tumblr, the Post.

A post should have the following attributes:

- `content` - Text belonging to the post
- `creatorId` - ObjectId of the post's creator
- `picPath` - Where the picture is stored
- `picName` - The picture's name

For this iteration you must create the **model**, along with the **new**, **create**, **show** and **index** routes. This should include file uploading.

A user should be logged in to create a post, but _not_ to view.

The **index** will be the home page, and simply display all of the posts on the website.

### Iteration 3 | Comments

Posts have comments attached to them. Create the Comment model as a subdocument of the Post.

A comment _can_ have images attached to it, but not all do.

The model should have the following attributes:

- `content`
- `authorId`
- `imagePath`
- `imageName`

You should create routes to create new comments. Comments should be displayed on the Post _show_ page.

Happy Coding 💙
