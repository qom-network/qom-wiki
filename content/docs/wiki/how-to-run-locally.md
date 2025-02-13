---
title: Run the site locally
type: docs
prev: docs/wiki
next: 
---

### Pre-requisites
---
- [Git](https://git-scm.com)
- [Go](https://golang.org/doc/install)
- [Hugo](https://gohugo.io/getting-started/installing/)

*Note: Make sure you have installed all the required tools before proceeding.*



### Run the site locally
---
#### Step 1
Clone the repository on your local machine and navigate to the project directory.
```shell
# Clone the repo to your local machine
git clone https://github.com/qom-network/qom-wiki.git

# Navigate to the project directory
cd qom-wiki
```

#### Step 2
Install required modules
```shell
hugo mod tidy
```

#### Step 3
Start the Hugo server on development mode. ( Do it each time you wanna launch your local site to work on it ) 
```shell
hugo server
```
This will start a local server on port 1313, and you can access the site at [http://localhost:1313](http://localhost:1313).

You can now make changes to the site and see them live on the server. The server will keep running until you stop it manually ( Press Ctrl+C to stop ).

### How I could edit it?

I recommend you use [Obsidian](https://obsidian.md), which is a local markdown file editor.

You can open the repository with this editor and you will be able to see your changes in real time both in the editor and in your browser (if you executed the command above that starts the local server).

### Which files could I edit?
---
**Content**:  All the content data is in the `content` directory. You can edit the markdown files in this directory to make changes to the site content, feel free to add new markdown files as well, organizing them in subdirectories, linking to them from other pages, etc.
  
* This site is powered by the Hextra Template, for more information about how to configure it, visit: [Hextra](https://imfing.github.io/hextra/docs/).
* The universal format used throughout the content is [Markdown](https://www.markdownguide.org).

**Root files**: All the configuration files are in the root directory. **We should not edit these files unless we know what we are doing**.

### How can I push my changes to the main repository

We are working on writing detailed instructions so that they are easy to use for everyone...

In the meantime:
#### If you are familiar with git and github
1. In your github account, create a branch of your own with your changes.
2. Create a Pull-Request pointing to our main branch.
3. The Pull-Request will be reviewed (only to review very obvious things like bugs, or to avoid malicious information)
4.  Once the Pull-Request is approved by the community, your changes will be live on the site.

#### If you want help uploading your changes

Contact to [RED](https://t.me/teh_woman_in_red) on telegram, send her your files and she will help you upload them.