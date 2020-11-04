# How to host a resume on GitHub Pages
> By [Ayush Patel](https://github.com/Ayush393/Ayush393.github.io) 

This **README** file describes the practical steps of how to host and format a resume using Markdown, a Markdown editor, GitHub Pages and Jekyl. It will also relate the practical steps to the general principles of current Technical Writing, as explained in Andrew Etter’s book Modern Technical Writing.

## Table of contents

- [Audience](#audience)
- [Purpose](#purpose)
- [Prerequisites](#prerequisites)
- [Instructions](#instructions)
- [Authors and Acknowledgements](#authors-and-acknowledgements)
- [FAQs](#faqs)

# Audience
This README is for computer science students who look forward to hosting their resumes in a static website using Jekyll, Markdown and Github Pages.

# Purpose

This README's purpose is to describe the practical steps of how to host and format a resume using Markdown, a Markdown editor, Github Pages and Jekyll with reference to Andrew Etter's book *Modern Technical Writing*. 

# Prerequisites
> According to Etter's book he emphasizes on the use of Lightweight Markup Languages since they are easy to learn and make it easy to read in its raw form.
1. A Github account.
2. A resume formatted in Markdown to enable you to get started on the practical steps to host it on the github page.

See [more resources](#more-resources) for a link to a good Markdown tutorial in order to create your resume in a Markdown Editor.

# Instructions
### Creating a Github account and repository
> GitHub is a code hosting platform for version control and collaboration. It lets you and others work together on projects from anywhere. This [tutorial](https://guides.github.com/activities/hello-world/) teaches you GitHub essentials like repositories, branches, commits, and Pull Requests. According to Etter's book it also encourages developers to contribute.

1. Go to [GitHub](https://github.com/join) and create an account.
2. Create a new GitHub repository [here](https://github.com/new).

### Building your Static Website
>  According to Andrew Etter "Static websites have no server side application dependencies, no databases and nothing to install so migrating an entire site is as easy as moving a directory. Because all it has to do is serve pages and the server needs very few hardware resources. Also you can host static websites practically anywhere. The basics are that you provide a static site generator with content (lightweight markup) and a theme (templated HTML and CSS), and it processes everything into a working website." Therefore, to create a working static website we simply need to modify the Markdown files.  
#### 1. Forking a resume template/theme
Forking means making a copy of a repository that allows you to freely experiment with changes without affecting the original project.

You can search for templates that are supported entirely by Github pages and powered by Jekyll over the internet. Some of them that inspired me are:
1. [Beautiful Jekyll](https://github.com/daattali/beautiful-jekyll)
2. [Modern Resume Theme](https://github.com/sproogen/modern-resume-theme)

To do this, you can simply click on the __*Fork*__ button at the top right corner of the page.
In my case I preferred forking the [*Modern Resume Theme*](https://github.com/sproogen/modern-resume-theme). 

If you choose to download and extract the zip file into the git repository you have just created instead of *forking* it, and edited it on your desktop, you can commit and push the resume template to Github.

3. Commit and push the resume template to github

```
$ git add --all
$ git commit -m "Initial resume setup"
$ git push -u origin master
```

#### 2. Rename the repository to `<yourusername>.github.io`
Click on __*Settings*__ at the top (the cog icon) and on that page you'll have an option to rename the project (*Repository name*). This will create a website with the **Modern Resume Theme** template that will be available at `https://<yourusername>.github.io` within a couple minutes. The repository must be renamed as username and no other name, otherwise Github pages will not recognize it as a website. Check out [FAQs](#faqs).

#### 3. Modifying the resume Template
Edit the `_config.yml` file `front matter` to modify and add content of your own resume. 
1. To edit the file, click on it to view the file and then click on the __*pencil*__ icon to edit it.
2. It will also allow you to change the titles of some of the content sections. 

#### 4. Viewing the website
1. Go to your GitHub repository settings.
2. Select the branch `master` under Source and select `Save`.
3. `https://<username>.github.io/` to view your static site.

Here is a demo featuring the resume in a GIF

![resume](/assets/resume.gif)

### More Resources

1. [Markdown Tutorial](https://helloacm.com/markdown-markup-language-quick-tutorial/)
2. [Andrew Etter's *Modern Technical Writing*](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS)
3. [Resume Template](https://github.com/sproogen/modern-resume-theme)
4. [Github tutorial](https://guides.github.com/activities/hello-world/)

# Authors and Acknowledgements

This resume theme/template powered by Jekyll and Github was inspired from [James Grant](https://github.com/sproogen/modern-resume-theme). This template provided with the easiest way to modify and use it for your own resume without any complication to be able to host it on your Github page. 

- Group members: Conner Kulbaski, Johnnus Gomez and Connor Bean. 

# FAQs
#### **Why is Markdown better than a word processor?**

- With Word you have tens or even hundreds of buttons to do different kinds of formatting. With Markdown it's much easier as it only supports limited features and you can easily learn the syntax in less than an hour. Limited features also means, most of the time, more readable and structured output.
- One of the best things is that you can edit Markdown files on any platform with the editor of your choice

#### **Why is my resume not showing up?**

1. Ensure your respository name is in the following format: `<username>.github.io`.
2. Ensure your repository's visibility is set to `Public`.
3. Ensure your GitHub Pages site is being built from the `master` branch.


