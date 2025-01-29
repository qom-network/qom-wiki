---
title: Run the site locally
type: docs
prev: docs/this-site
next: 
---

### Pre-requisites
---
- [Hugo](https://gohugo.io/getting-started/installing/)
- [Go](https://golang.org/doc/install)
- [Git](https://git-scm.com)


### Run the site locally
---
#### Step 1
Clone the repository on your local machine and navigate to the project directory.
```shell
# Clone the repo to your local machine
git clone https://github.com/qom-network/qom-docs.git

# Navigate to the project directory
cd qom-docs
```

#### Step 2
Install required modules
```shell
hugo mod tidy
```

#### Step 3
Start the Hugo server on development mode.
```shell
hugo server --logLevel debug --disableFastRender -p 1313
```
This will start a local server on port 1313, and you can access the site at [http://localhost:1313](http://localhost:1313).

You can now make changes to the site and see them live on the server. The server will keep running until you stop it manually ( Press Ctrl+C to stop ).


### Which files could I edit?
---
**Content**: All the content data is in the `content` directory. You can edit the markdown files in this directory to make changes to the site content, feel free to add new markdown files as well, organizing them in subdirectories, linking to them from other pages, etc.
  
* This site is powered by the Hextra Template, ror more information about how to configure it, visit: [Hextra](https://imfing.github.io/hextra/docs/).


**Root files**: The root files are the configuration files for the site. All the configuration files are in the root directory. **We should not edit these files unless we know what we are doing**.

