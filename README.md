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
    - Next, on the command line, navigate to the directory where you want your website to be located on your computer. Create a new folder.
    - Then run this command inside the new folder to create a website: **pelican-quickstart** (You will need to answer some intuitive questions during this process)
    - You should end up with these documents below or similar ones inside your website folder.
        ![Image 1](Screenshot 2025-03-06 190347.png)

  - ### Step 2 | RESUME FORMATTING
    - Using a text editor (e.g VS Code), format your resume with Markdown using headings to create sections, lists, font styles (bold, italic e.t.c). **Note:** Markdown cannot recreate the format of the resume exactly.
    - Save this Markdown file in the folder named **content** within your website folder.
    - 
