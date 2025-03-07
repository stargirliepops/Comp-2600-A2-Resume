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
- A Forge (that can host static websites and supports the DVCS you choose)

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
    - Then 
