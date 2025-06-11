# Steal this Site

Welcome to **Steal this Site** – a blueprint for building your own personal website with **Astro** as a wrapper and **React** components for interactivity. Inspired by the ethos of *Steal This Book*, this project is yours to fork, adapt, and make your own.

---

## Who is this for?

- **Tinkerers and Makers** – If you love learning by doing, this is a perfect starting point.  
- **New Coders** - Working on this project will help you get from "I know HTML" to "I know how to launch a modern webpage".
- **People Who Want a Minimalist Personal Site** - A clutter free landing page on the internet that YOU built, YOUR way.
- **Anyone Interested in Docs-as-Code** - Technical writers, engineers, project managers... whoever you are and whatever you make, leave the Word files behind. 

In short, this is for **anyone** regardless of programming skill who wants to start small, learn enough to be dangerous, and make your own corner of the Internet.

---

## What's Inside

This repo contains: 

- A *mininalist* **Astro** site skeleton
- A few simple **React** components (for our *Hero*, *About*, *Contact*, and other sections)
- **Tailwind CSS** for styling
- **AsciiDoc documentation** (`/docs/`) – project-specific docs: usage, customization, deployment 

---

## Highlights

- Fully documented in AsciiDoc for Docs-as-Code best practices  
- Clear, easy-to-follow project structure – perfect for learning and tinkering  
- Interactive **React** components wrapped in static **Astro** pages  
- **Ready to deploy** to **GitHub Pages** or **Netlify** with minimal configuration  
- Designed for easy forking and adaptation – start with this and make it your own!

Here's what the project file structure looks like:

```
steal-this-site/
├── src/                  # Site code (Astro pages & React components)
│   ├── pages/
│   ├── components/
│   └── styles/
├── docs/                 # Project documentation in AsciiDoc
├── public/               # Static assets
├── netlify.toml          # Optional Netlify config
├── package.json          # Project dependencies
├── README.md             # This file
└── LICENSE               # MIT License
```

--- 

## Some Terminal Advice

To get the most out of this project, you'll need to be comfortable using the **terminal**, or command line interface.

You'll be using the terminal to:
- Clone this repo with **Git**
- Install dependencies with **pnpm**
- Run the local development server (Astro)
- Deploy your code to platforms like **GitHub Pages** or **Neflify**

**Mac/Linux users** – You’re probably already familiar with the terminal (Terminal.app, iTerm, etc.).  

**Windows users** – We recommend using **Windows Subsystem for Linux (WSL)** for a smoother experience. While it is possible to perform these tasks using **PowerShell** or **Command Prompt**, you'll have a much smoother experience if you choose to use WSL because it gives you a *real* Linux bottled environment inside of Windows where modern web tools (Astro, Node, etc.) work exactly as intended, without clunky workarounds.

  [Here’s a quick guide to installing WSL](https://learn.microsoft.com/en-us/windows/wsl/install).

---

## Tools You'll Need

To complete this project, you'll need the following:

- **Visual Code Studio** - [VSCode](https://code.visualstudio.com/) is a powerful, user-friendly, and free code editor produced by Microsoft. It has a great community of developers who provide extentions for working with just about every programming language/framework/et cetera you can think of. If you think VSCode isn't for you, take a look at some alternatives and pick a code editor you vibe with the most.

- **Node.js** - The JavaScript runtime environment that powers Astro and React. Node allows you to run JavaScript tools like build scripts and servers outside of a browser. Whenever you install packages (see: pnpm), or run a development server, that's Node working in the background. Install guide: [Node.js](https://nodejs.org/).

- **pnpm** - This project uses pnpm as its *package manager*, or, the tool that manages the *software libraries* our project depends on. "What's a software library?" Software libraries, also called *dependencies* are pre-written code meant to solve common problems like creating interactive user interfaces (**React**), page stying (**Tailwind CSS**), or building static webpages (**Astro**). Rather than writing all that code from scratch, modern developers can simply install these *building blocks* into your project and use them where and how you'd like.

  The *package manager* is the tool that handles all that for you, it: 
  - *Downloads* these libraries from the **npm registry** (a huge warehouse of open-source code)
  - *Keeps track* of what versions your project uses so updates don't break anything
  - *Organizes* these libraries in a folder called `node_modules/` so the developer doesn't have to worry about anything
  - *Removes* those libraries cleanly when your done with them
   
    Later, when you run the command `pnpm install` in the terminal, you're telling the package manager to fetch all the libraries your project relies on. [Official pnpm Install Guide](https://pnpm.io/installation).

- **Git** is an example of a *distributed version control system (VCS)*, created by Linus Torvalds (the creator of Linux) in 2005, it has become a *foundational technology* in software development. Basically, Git tracks changes in a code base by creating **commits** or *snapshots* that capture whatever changes that have been made since the last commit in what's called a **repository** or **repo** . If you make a change and it breaks your program, you can simply *revert* back to an earlier commit when everything was working properly. If you want to try something new, you can create a **branch** - a parallel version of your project - and **merge** those changes back into your main code later if desired. Install guide: [Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git).

- **GitHub** is the cloud-based home for your Git repo. It’s built around Git but adds a powerful layer of tools for collaboration, discussion, and sharing.

  GitHub:
  - **Hosts your code**, allowing you to share your project with the world.
  - **Tracks issues**, helping you manage bugs, tasks, and improvements.
  - **Reviews changes**, enabling you to propose updates and collaborate with teammates through pull requests.
  - **Deploys directly**, making it easy to publish your site with services like Netlify and GitHub Pages.

  Joining GitHub means joining a larger world of developers—people who share, fork, remix, and collaborate to build better software together.

  If you’re new to GitHub, it’s free to join and has tons of resources to help you get started: [GitHub Sign Up](https://github.com/).

- The Terminal – Your command center, where you’ll run build commands and deploy your site.

  💡 I personally use the built-in terminal in VSCode—it’s convenient and works the same across Mac, Linux, and Windows (with WSL).

---

## Why this workflow matters

This workflow—cloning the code, running it locally, and deploying it to Netlify—mirrors how real-world development and deployment work. It’s a simple but powerful process that lets you test and tweak your changes safely before sharing them with the world. By following these steps, you’re not just setting up a personal site—you’re learning the same process used by professional developers every day.

---

## Getting Started

1. Clone the Repo
   git clone https://github.com/yourusername/steal-this-site.git
   cd steal-this-site

2. Install Dependencies
   pnpm install

3. Start the Dev Server
   pnpm dev

4. Deploy
   See detailed instructions in docs/deployment.adoc for GitHub Pages and Netlify deployment.

Here’s how these steps fit together:

```
1. Clone the repo
   git clone ...

       ↓

2. Install dependencies
   pnpm install

       ↓

3. Run locally
   pnpm dev

       ↓

4. Deploy
   Push to GitHub
   Connect to Netlify / GitHub Pages
```



---

## Docs-as-Code

This project includes a /docs/ folder with project-specific documentation in AsciiDoc.  
It covers usage instructions, customization tips, and deployment steps for this starter site.

---

## License

This project is licensed under the MIT License – see the LICENSE file for details. Fork it, remix it, and make it your own!

---

## Let’s Collaborate

Have ideas or want to suggest improvements?  
- Open an issue  
- Create a pull request  
- Or just fork and remix it!

---

Happy hacking, and remember: this site is yours to steal, adapt, and grow.

— Dom Caracappa


