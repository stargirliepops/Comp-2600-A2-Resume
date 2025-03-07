# STATIC WEBSITE CREATION (FOR A RESUME) AND HOSTING THE WEBSITE ON A FORGE 
**This document describes the process for creating, formatting, and hosting a resume**
**This document is for anyone who is interested in learning more about a Distributed Version Control System (DVCS), static site generator or forges. They should typically have a basic understanding of how to use Markdown and the command line.**

## PREREQUISITES
#### What you will need to carry out the instructions
- A Resume
- Knowledge of Markdown (headings, lists, bold, italics, links & images)
- A Text Editor (I used **VS Code** to write the Markdown file(s) for my website, you can download the text editor for your operating system here: [Install VS Code](https://code.visualstudio.com/download))
- A Distributed Version Control System (I used Git for my website's files)
- A Static Site Generator (I used Python-based Pelican - it supports Markdown)
- A Forge (To host the static website and that supports the DVCS you choose. I used GitHub.)

## INSTRUCTIONS
#### A guide for you
  
  - ### Step 1 | GENERATING YOUR STATIC WEBSITE
    - Install Python: [Python](https://www.python.org/)
    - On the command line, install Pelican by running this command: **python -m pip install "pelican[markdown]"**
    - Next, on the command line, navigate to the directory where you want your website to be located on your computer.
    - Now, create a new folder.
    - Then run this command inside the new folder to create a website: **pelican-quickstart** (You will need to answer some intuitive questions during this process)
    - You should end up with these documents below or similar ones inside your website folder.
        ![Image 1](Image1.png)

  - ### Step 2 | RESUME FORMATTING
    - Using a text editor (e.g VS Code), format your resume with Markdown using headings to create sections, lists, font styles (bold, italic e.t.c). **Note:** Markdown cannot recreate the format of the resume exactly.
    - At the top of your Markdown document, include these attributes changing the **Title** and **Date** ![Image 2](Image2.png)
    - Save your Markdown file in the folder named **content** within your website folder.

  - ### Step 3 | ADDING YOUR RESUME TO YOUR WEBSITE
    - To turn your resume to a website, Pelican converts the Markdown file into HTML.
    - To do this, on the command line (in your website's folder) run **pelican content**

  - ### Step 4 | VIEWING YOUR WEBSITE IN YOUR BROWSER
    - To view your static website on your computer, go to the command line and run **pelican --listen**
    - After that, you should see this on the command line: ![Image 3](Image3.png)
    - Ctrl + click on the link to open your website in your browser.
   
  - ### Step 5 | HOSTING YOUR WEBSITE ON A FORGE
    ##### You need other people to be able to view your website on the internet and to do that, you need to host your site using a forge. For this project, we will use GitHub.
    
      - #### Step A: Creating a new repository on GitHub
        - First, on the command line run this command to install ghp-import: **python -m pip install ghp-import**
        - Next, install your DVCS (in this case, Git) using this link: [Git](https://git-scm.com/)
        - Now, if create an account on GitHib, if you do not already have one : [GitHub](https://github.com/)
        - After creating your GitHub account, create a new repository, set it to **public**, and name it appropraitely
          
      - #### Step B: Setting up your GitHub Project
        - You will need to store your GitHub repository on your computer. This is called *cloning*.
        - To clone your repository, navigate on the command line to a folder where you want this repository stored
        - Then run this on the command line: git clone https://github.com/yourGitHubusername/nameofyourrepository.git
        - Recall the website folder you created earlier, now move it into this cloned repository on your computer (you should see files like in the image in your cloned repository) ![Image 4](Image4.png)
        - Next, commit to GitHub by running these on the command line:
            1. git add .
            2. git commit -am "First commit"
        - Generate the website and send your site to your GitHub repository (under the section called *Pages* by running these on the command line:
            1. pelican content -s publishconf.py
            2. ghp-import output -b gh-pages
            3. git push origin gh-pages
        - Lastly, in your GitHub repository, click on *Settings*
        - Then navigate to a section called *Pages*
        - Click on the link to your website shown on this page. It should look like this: ![Image 5](Image5.png)

#### Now you have a public static website. Yay! 🎉
   
        

