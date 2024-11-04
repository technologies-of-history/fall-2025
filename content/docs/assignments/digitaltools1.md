---
layout: page
bookTOC: false
draft: false
title: Digital Tools 1
---
# Communicating Simply with Markdown, Hugo, and GitHub
By now you've created a [GitHub](https://github.com) account, practiced opening a repository, making changes to a file, making a pull request, and merging branches with GitHub's [Hello World](https://guides.github.com/activities/hello-world/) tutorial. You've followed the [Markdown lesson](https://programminghistorian.org/en/lessons/getting-started-with-markdown) on the Programming Historian, so you know how to style your text files with Markdown syntax. We've practiced authoring Markdown files in class, but now it's time to do it on your own and create content for our course blog. You'll be following these same steps to create and submit the rest of your Digital Tools assignments, so it's very important for you to get the hang of these basic steps now.

## Step 1: Think about downloading a text editor

All of your digital assignments this semester will be authored in Markdown, which means 
you can't use Google Docs or Microsoft word to create them. As you know, you can always 
create Markdown files (.md) directly in GitHub, but if you'd like to be able to complete 
your assignments offline, save your work on your own machine, and preview your work in a 
local development environment on Hugo, then you will want to use a text editing program to 
write and save your .md files. If you've done some programming/coding 
before, you likely already have a favorite text editor, and you should keep using it. If not, 
I really like [BBEdit](https://www.barebones.com/products/bbedit/) for MacOS 
and [Notepad++](https://notepad-plus-plus.org) for Windows. Both provide nice features in their
"free" mode, and don't require a subscription.

## Step 2: Take a look at an existing post

Open the class repository that you've forked into your personal GitHub account. Find the **posts** 
folder and open it. You'll see a single file in there titled **2020-11-15-Welcome to Technologies of History.md**. 
This is the Markdown file for the blog post that appears on the homepage of our course website. 
Note the file naming conventions. All of the blog posts created for our site must be named 
in the same way: **yyyy-mm-dd-your title.md**.

Click the name of the file to open it, and then click on the pencil icon in the upper right 
to edit the file. You should now see the post written in Markdown with a header at the top 
that looks like this:

 ```
 ---
 layout: post
 author: Melissa Reynolds
 bookTOC: false
 draft: false
 title: Welcome to Technologies of History
 ---
 ```

Note the formatting of this file. The heading at the top is very important. Every post that 
you write for our course site must include this same header, though of course you'll change 
whatever comes after the "title" field to your chosen title. Without the header, Hugo 
doesn't know to turn your Markdown file into a webpage.

Here's what this header is telling Hugo:

``layout: post``  This is a post, not a static webpage, and should display with author and date information and be sorted on the homepage with most recent at the top.  

``author: Melissa Reynolds``  Hugo knows to include this name as the author in the metadata and header of this post.  

``bookTOC: false`` The template we're using in this class has an option to include a left-hand menu that is automatically populated with the any header text. I've opted to switch this off, but if you want it, change the code to read ``bookTOC: true``  

``draft: false`` This tells Hugo that this post is no longer a draft and is ready to be served to the website. The absence of this piece of code or ``draft: true`` tells Hugo that the post isn't ready to go live yet.  

``title: Your Title Here`` This one is pretty self explanatory!


## Step 5: Write a new post in Markdown

Now complete your assignment: write a 2–3 paragraph post reflecting on the relationship between the
nature or format of a communication technology and the kind of knowledge that technology can
produce. Historians have suggested, for example, that alphabetic writing enabled 
the development of philosophical thought in Greece that was markedly different from that of ancient
Mesopotamia, with its cuneiform syllabary. In what ways do we see a similar relationship between
the principles of static computing and the production of digital scholarship? Are historians
arguments constrained or shaped by the tools they use to tell them?


(Note: the following instructions are for those of you brand new to GitHub, who don't use 
GitHub desktop or a text editor. This is the *most basic* 
way to add a file to your repository, but if you already know how to push changes and commit 
via those other platforms, go right ahead.)

__If you're writing directly in GitHub:__
1. Create a **New Branch** in our course repository. 
2. Click the arrow to the right of **master** in the branch menu, and in the search box type in the name of the new branch you'll create: **lastname-dt1**.
3. Click the option that appears that says **Create branch: lastname-dt1**.
4. Open the **posts** folder of that new branch. 
5. Click **Create New File** and create a new Markdown file with the appropriate naming conventions: **yyyy-mm-dd-your title.md**.
ALL posts you create for this course blog must follow these exact naming conventions.

__If you're writing your posts in a text editor:__
1. Open your text editor of choice and create a new reate a new Markdown file with the appropriate naming conventions: **yyyy-mm-dd-your title.md**. 


## Step 6: Commit your post

__If you're writing directly in GitHub:__
1. Click the green **Commit** button to save the post to your repository. 

__If you're writing your posts in a text editor:__
1. Create a **New Branch** in our course repository. 
2. Click the arrow to the right of **master** in the branch menu, and in the search box type in the name of the new branch you'll create: **lastname-dt1**. 
3. Click the option that appears that says **Create branch: yourname-dt1**.
4. Navigate to the **posts** folder and click **Add File** and then **Upload Files** and either drag and drop or select your Markdown file to upload. 
5. Then **Commit** that file to your repository as you would one authored directly in GitHub.

4. Upload your post into the **_posts** folder of the new branch. 
5. **Commit** your changes, and create a **Pull Request** to merge it with the **master** branch of our repository. **Pay attention** and be sure you select the right **head** for your request.



## Step 7: Create a pull request

You've written your post and committed it to your **posts** folder in your personal repository. 
Now, it's time to notify the developer (me) that you'd like the post to be merged into the **main** branch of the
site so that it can be served to the website.

1. In the menu at the top of your repository, click **Pull requests**. 
2. Click the green button **New pull request**. 
3. You'll now see a gray box at the top that shows you the **base** repository you'll be sending your changes to (digital-history/digital-history.github.io), and the **head** repository, which is yours **(digital-history/lastname-dt1)**. NOTE: Be sure that yours is the **head** and the main branch is the **base**.
4. Name your pull request **LastName_dt1** and then click **Create pull request**.

Ok, that's it! You've written a blog post in Markdown and followed the standard GitHub workflow to send it to our class site. Pat yourself on the back, and know that you'll do it all over again for the next three assignments.
