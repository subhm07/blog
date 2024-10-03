---
layout: post
title:   Doom Emacs (Day 1)
date: 2024-09-24 12:00:00
---

Doom is a configuration framework for GNU Emacs tailored for Emacs bankruptcy veterans who want less framework in their frameworks, a modicum of stability (and reproducibility) from their package manager, and the performance of a hand rolled config (or better). It can be a foundation for your own config or a resource for Emacs enthusiasts to learn more about our favorite operating system.

![_config.yml]({{ site.baseurl }}/images/evil.jpg)

I use Athena OS based on arch which is basically known for Redteam and Blueteam training preinstalled tools with themed windows manager like Bspwn, Xfce, Gnome etc. I've faced many issues with hanging around terminals and windows manager for my custom pentesting purposes. Doom emacs is not just a editor its much more then that like org or evil mode and specially buffer management  and finally something which i found enormously powerfull and accurate for day to day basis. I'll share my experience of using doom emacs and Lets me show some basics first :

# **Doom Emacs: The Ultimate Configuration Framework for Power Users**

Doom Emacs is taking the Emacs world by storm. But what exactly is it, and why are so many developers and power users flocking to it? If you're unfamiliar with Emacs, you might ask, "Isn’t Emacs that old, difficult-to-use text editor from the '80s?" Yes, but Emacs has evolved, and Doom Emacs brings a new level of customization, power, and usability to it. Let’s explore how Doom Emacs works and why it’s considered a game-changer for productivity, coding, and more.

## **What is Doom Emacs?**

Doom Emacs is a configuration framework designed to make Emacs more user-friendly and powerful. At its core, Doom Emacs is an optimized configuration for Emacs, created to make it easy to use out of the box. Think of it as a toolbox for transforming Emacs into a highly efficient, streamlined editor, especially for those who love a fast workflow and Vim-like keybindings.

Doom Emacs is built on top of vanilla Emacs and includes an extensive set of pre-configured modules. These modules allow users to activate features they need, like programming language support, UI improvements, and integrations with tools like Git. The main advantage? You don’t need to be an Emacs expert to get it working the way you want.

## **Why Should You Use Doom Emacs?**

The decision to use Doom Emacs comes down to one primary factor: customization without the hassle. It offers several key benefits:

- **Pre-configured Modules:** Doom Emacs comes with a vast array of modules that can be enabled or disabled to tailor your experience. Need a Python development environment? Just activate the Python module. Want Git integration? Turn on Magit. There’s no need to manually configure every feature.
  
- **Performance Boost:** Doom Emacs is optimized for speed, boasting faster startup times and leaner memory consumption compared to vanilla Emacs. This makes it a great choice for developers who work with large files or complex projects.

- **Vim Keybindings (Evil Mode):** One of the most significant advantages is Doom Emacs' use of Evil mode, which integrates Vim keybindings into Emacs. This gives users the best of both worlds — Emacs' flexibility and Vim’s efficient text editing commands.

- **Community-Driven:** Doom Emacs has a vibrant community that continuously contributes to its development. If you run into any issues, there’s an active support network that can help you troubleshoot.

## **How to Get Started with Doom Emacs**

Getting started with Doom Emacs might sound intimidating, but it’s surprisingly straightforward. Here’s a basic roadmap to get you up and running:

1. **Install Emacs:** If you don’t have Emacs installed yet, you’ll need to install it first. You can easily install it on Linux using:
   ```bash
   sudo apt install emacs
On macOS, use Homebrew:

bash
Copy code
brew install emacs
On Windows, download it from the GNU Emacs website and follow the installation instructions.

Clone Doom Emacs: Once Emacs is installed, open a terminal and clone the Doom Emacs repository:

bash
Copy code
git clone https://github.com/doomemacs/doomemacs ~/.emacs.d
Install Doom Emacs: Run the following command to install Doom and generate the necessary files:

bash
Copy code
~/.emacs.d/bin/doom install
This will walk you through a few setup questions and build your initial configuration.

Configure Doom: Doom Emacs’ configuration lives in the ~/.doom.d/ directory. From here, you can customize modules, keybindings, and packages by editing the init.el, config.el, and packages.el files. For example, to enable Python development, you would uncomment the Python section in init.el.

Sync Your Configuration: After making any changes to your configuration, run:

bash
Copy code
doom sync
This applies your changes and keeps your Emacs environment up to date.

Key Features and Modules of Doom Emacs
What truly sets Doom Emacs apart is its modular approach. Here are some of the most popular modules that you might want to enable:

Completion Systems: Doom offers robust completion systems like ivy or helm with fuzzy searching to help you find files, buffers, and commands quickly.

UI Enhancements: From slick modelines to clean themes, Doom improves Emacs’ interface significantly. The doom-themes module gives you access to beautiful color schemes.

Language Support: Whether you're working with Python, JavaScript, C++, or even Markdown, Doom has a module for it. The lsp module integrates the Language Server Protocol, making Doom Emacs a powerful IDE.

Version Control with Magit: Magit is arguably the best Git interface available, and it’s seamlessly integrated into Doom Emacs. Stage, commit, and push with ease using intuitive keybindings.

Customizing Your Workflow with Doom Emacs
One of the best parts about Doom Emacs is that it’s highly customizable. From remapping keybindings to integrating external tools, Doom can adapt to your workflow. Here’s how to take your Doom Emacs experience to the next level:

Personal Keybindings: You can add custom keybindings to make Doom fit your style. For example, if you want to bind SPC o f to open a specific file, you can add the following in your config.el:

elisp
Copy code
(map! :leader
      :desc "Open my file" "o f" #'find-file)
Package Management: Need additional functionality? You can easily install new packages. Add them to ~/.doom.d/packages.el and run doom sync. For example, to install flycheck for syntax checking:

elisp
Copy code
(package! flycheck)
Doom Emacs vs. Other Editors
How does Doom Emacs compare to other popular editors like VSCode or Atom? It boils down to the following points:

Speed: Doom Emacs is faster, especially when working with large codebases, thanks to its performance optimizations.

Customization: Doom allows for far deeper customization than other editors. Whether you want to tweak aesthetics, behavior, or workflow, you can change almost anything.

Vim Keybindings: While some editors support Vim keybindings, Doom Emacs’ Evil mode offers the most seamless Vim integration, perfect for developers who want Vim efficiency with Emacs' power.

Conclusion: Should You Switch to Doom Emacs?
So, is Doom Emacs for you? If you’re a power user who enjoys customization and efficiency, the answer is likely yes. Doom Emacs gives you the flexibility of Emacs with the speed and convenience of a modern editor, all while allowing you to customize your workflow to fit your needs.

However, if you're someone who prefers simplicity over customization or doesn’t have time to learn keybindings and configuration, you might want to stick with a more beginner-friendly editor.

Ultimately, Doom Emacs is more than just a tool; it’s an investment in productivity and customization. Are you ready to take control of your editing environment and unlock a more powerful way of working?



