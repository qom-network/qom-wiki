---
title: Way to launch your site 🦅
type: docs
prev: 
next: 
sidebar:
  open: true
---


## 1️⃣  **Install BabelFish**
  
### Installers - Public Drive:  
 > [BabelFish v1.0.2(For Mac and Windows):](https://drive.proton.me/urls/JQW9RTSNRG#AyMTHvghfSTc)

> [!warning]**hash SHA-256 of each file**:
>
> ef039682586b94b73c45213b02765a943f8b3e0068c46cd3dcc61fb63e35ff01  (BabelFish-v1.0.2-MacOS-App.dmg)
>
> 90227fe60bdfe80674d9ed13b580fb99371a43a4a2c9c34cfffff8564595f8a8  (BabelFish-v1.0.2-MacOS-Installer.dmg)
>
> a76e2e765b487e03fe8f3a179ba26ea0f6d97bdf5e8083e0afa29724bb664dc8  (BabelFish-v1.0.2-Windows.exe)
>   
> -----
> 
> *This is the 'exact size' of the files; if you calculate the hash of any of these files on your computer, you should get the exact string as described here.
> This is to validate that you are receiving the exact file without modifications along the way.
>
>
> To calculate it on mac:
>
> ```
> shasum -a 256 BabelFish-v1.0.2-MacOS-Installer.dmg
> ```
>
> To calculate ir on windows
>
> ```
> certutil -hashfile BabelFish-v1.0.2-Windows.exe SHA256
> 
> ```
> **teh_woman_in_red**


> [!IMPORTANT] 🍎 **Mac Setting** 
>
> Go to "*Settings*" -> "*Privacy & Security*"  
>   
> and select "*Allow apps downloaded from: App Store and identified developers*"  
>   
> then click "*Open Anyway*"
  


- After installing Babelfish, **turn on the buttons and Check if you can access `.qom` domain websites:**  
> http://hello-world.qom

> [!IMPORTANT] **Windows setting**
>
> 1. *Uncheck TCP/IPv6*  
> 2. *Manually set the IPv4 DNS server to 127.3.6.9*  
  


---

## 2️⃣ Fork the Hello World repository from GitHub and set up GitHub Pages

If you're new to GitHub, please complete registration and initial setup using a [**Beginner’s guide**](../gitguide) before proceeding to the next steps.


> **Hello-World Repository:**  
> https://github.com/deep-thought-computer/hello-world

Follow the *steps 1–3 in the `README.md`* of the repository to fork it and set up GitHub Pages. (Step 4 will be explained later.)

---

## 3️⃣ Inform us your GitHub Pages URL and preferred domain name

Once you've successfully set up your GitHub Pages URL in Step 2, *contact the developer with your desired `.qom` domain name.*

After your domain is issued, you’ll likely be greeted by the familiar **"Hey!"** waving uncle when you access it.

Currently, we are in the testing phase. To obtain a `.qom` domain, please contact a developer. After the testing phase, domain names will be mintable as NFTs.

---

## 4️⃣ Build Your Website

Now that you’ve forked the repository, you are free to add your own code and files to build your site. If you already know how to do this, go ahead! However, for ongoing development, **we recommend using the tools below.** Any changes you push to GitHub will automatically update your site after about 5 minutes.

If you're unfamiliar with building websites and unsure what to do next, the following guide will help you get started. We also recommend becoming familiar with the tools introduced below.

> ### 4. Normal Workflow
> ```bash
> # To fully edit your repository, clone it locally using:  
> git clone https://github.com/your-user-name/hello-world.git
> 
> # Edit files (e.g., `index.html`), then run:  
> git add .  
> git commit -m "Update"  
> git push origin main
> 
> # Each push will automatically update your site at:  
> `https://your-user-name.github.io/hello-world`
> ```

---

## 🛠️Recommended Tools

### **📝 Code Editor**
Use a code editor to modify files. Any editor is fine, but [**Visual Studio Code**](https://code.visualstudio.com/) is recommended due to its free extensions and ease of use.

You’ll also begin using Terminal or PowerShell more frequently as development progresses. If you're unfamiliar with command-line tools, check out a basic [**CLI tutorial**](../howtousecli) 

---

### **💻 HUGO**
One of the most popular open-source static site generators, HUGO allows you to build fast and flexible websites.

Start by reading the official Quick Start Guide to get familiar with it. If you’ve already learned to use `git clone` and basic command-line operations, installation should be straightforward.

> **Quick Start Guide:**  
>  *https://gohugo.io/getting-started/quick-start/*  
>  For theme-specific instructions, refer to the theme’s `README`.
>
<!-- > Related article: [*2025-06-21-1050*](/posts/2025/06/2025-06-21-1050/) -->

Once you're done with the guide, choose a template theme and try customizing it. When you’re satisfied, move into your project directory and build the site with the `hugo` command.

**Copy everything in the generated `public` folder into your cloned `hello-world` directory, then run:**  

```bash
 git add .  
 git commit -m "Update"  
 git push origin main
```

---

### **🔮Obsidian**
[**Obsidian**](https://obsidian.md/) is a powerful local note-taking and knowledge management tool based on Markdown. It works seamlessly with HUGO and allows you to link notes freely.

It’s not only useful for editing Markdown files but also for personal knowledge management (PKM) and the Zettelkasten method.

There are many excellent open-source plugins available to extend its functionality.

> **Editing Toolbar**  
> A plugin that assists with Markdown syntax. You won’t need to memorize formatting rules.
> 
> **Smart Connections**  
> Uses AI to analyze the content of your notes and suggest links based on relevance.
