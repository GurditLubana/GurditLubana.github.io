
# Title: **Hosting a Resume on a public GitHub Repository**
 

# **Purpose**
The basic purpose of this Readme file is to list the practical steps of how to host and format a resume using Markdown by relating them to the general principles of current Technical Writing mentioned by Andrew Etter in his book "_Modern Technical Writing_".
****
# Prerequisites
To build and host the resume successfully, we would need some knowledge of Markdown language, a GitHub account, and a Markdown editor like- VS code. I have attached a link to the Markdown tutorial in the "More resources" section if you don't have any knowledge of Markdown. 
# Instructions

## **Use Distributed Version Control**

There are many reasons why most people today give preferance to Distributed version control systems like Git or Mercurial than other centralized systems. Some of those reasons includes:
- DVCS have better performance.
- It doesn't require any internet connection.
- It is superior for concurrent work.

>It is always recommended to save all your documentations in the same repository as its corresponding product source code, because by doing this:

- All the documentaions and code branches stay synced.
- Developers don't have to clone a seperate repository everytime, which leads to increase in their contributions. 

>However, there are some disadvantages to it as well:

- Building whole documentations could be a slow process, if the size of repository in large. 
- Even very simple documentations results in changing a chore, while performing commit hooks and pull request submissions.

In order to host our markdown resume on a website, we are going to use GitHub pages. After that, perform following tasks:

1. For that login to your GitHub account or _create an account_ if your account doesn't already existed. 
2. Now create a new repository and name it as:

```
GitHubName.github.io
```

## **Make Static Websites**

There are few reasons why Andrew Etter likes static websites, like:

1. Since there is no server-side application dependencies,installation or database involved, migrating whole site is not so hard to do. 
2. You can test Static websites from any local computer, without even installing any external application. 
3. It can never be hacked, spamed or crashed. 

### Hosting a Static Website Procedure

There are couple of steps that needs to be followed in order to host a website. 

1. First a software called Ruby needs to be downloaded and installed , if the system doesn't have it already. In order to download it, perform following actions:
    - Click on the link that has been provided in the "More Resources" section.
    - Click on RubyInstaller for windows or MacOs.
    - Click on the latest version of the RubyInstaller.
    - Now, click on the _Download_ on the left bottom side of the screen _(underneath RubyInstaller)_
    - Now, click on the WITH DEVKIT, and downloading will be started.
    - Once it get downloaded, open the application and install it, after accepting the terms and conditions. 

2. Now, a static site generator needs to be installed. To do, open command prompt and type _`gem installer bundler jekyll`_, and let it finish installing.

3. Now, download Git desktop and login using your GitHub account. Once you are logged in, perform following tasks:
    -   Open _File_ from the top left, and click _"clone repository"_.
    - Select the repository that you created, and choose the path where you want to clone that repository on your system. Click _clone_ after that.
    - Now, go back to the _Git Desktop_ and hit publish the branch and then click _Fetch origin_. 

4. Now we need to host our website on GitHub. In order to do that:
-  Open command prompt and select a directory where you want your local website.
- Now, type these commands one after another

    ```
     jekyll new Name-of-your-site
     cd Name-of-your-site
    bundle exec jekyll serve
    ```

5. Now go back to your directory where you created your website. You will find a directory titled `Name-of-your-site` in this folder you will find a file titled:

    ```
    index.mardown
    ```
    Open this file and copy and paste your markdown resume's code to this file, under three ---, save and close the file.

6. Now, since you repository is empty, copy all the folders from you website directory from Step 5, and paste them in your repository. Also copy and paste your readme.md file in this folder. 

7. You can now view your resume website at:
    ```
    GitHubName.github.io
    ```

## More Resources

- [Click here](https://rubyinstaller.org/) to find the Ruby Installer.
- [Click here](https://www.markdowntutorial.com/), if you want to learn how to use Markdown. 
- [Click here](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS), to purchase the Andrew Etter's book "_Modern Technical Writing_" from Amazon.

# Authors and Acknowledgements

- This Readme file was created by Gurdit Singh.
- Thanks to my group members for their feedbacks:
    1.  Muhammad Ibrahim
    2. Jacob Broggy 
    3.  Joseph Gonzales
- Andrew Etter's book "_Modern Technical Writing_"

# FAQs

Q1. Do you think Mardown is better than Latex, for resume building.\
> Yes, Latex is sort of sub set of Mardown language. Latex was made up from Markdown. But Mardown language is easier to understand and write. It is similar to writing a plain word doc with some extra features. However, you have to learn the complex syntax of overleaf, in order to be working with latex. 

Q2. Why is my resume not showing up?
> Usually server takes some time to get updated, so try waiting. It still doesn't show up make sure you have your resume pasted in index.markdown file.
