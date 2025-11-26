---
layout: '../../layouts/ProjTemplate.astro'
title: 'Portfolio'
description: 'A deep dive into how I built this personal portfolio using Astro, TypeScript, and GitHub Actions for CI/CD.'
publishDate: 'Oct 30, 2025' 
---

# Project: This Portfolio

Welcome to the most "meta" project on my site! This post is all about the very portfolio you're looking at right now. My goal was to build a fast, modern, and content-focused website to showcase my projects and share my thoughts.

After exploring different options, I landed on a powerful combination of technologies: **Astro**, **TypeScript**, and **GitHub Actions**.

![GitHub Actions Image](../../../public/assets/portfolio/githubactions.png)
*GitHub Actions Workflow history*


---

### Why Astro? 🚀

The biggest decision for this project was the framework. I chose [Astro](https://astro.build/) for a few key reasons:   

* **Performance First:** Astro is a static-site generator that ships **zero JavaScript by default**. This means my site loads incredibly fast, scoring top marks on performance metrics and providing a great user experience.
* **Astro Islands:** This is Astro's "secret sauce." It allows me to create interactive UI components (like a mobile menu or a theme toggle) that load their own JavaScript *only when needed*, without slowing down the rest of the page. This keeps the site snappy while still allowing for rich interactivity.
* **Content-Driven:** Astro is built for content. Its file-based routing and first-class support for Markdown (like this very post!) make it a perfect fit for a blog or portfolio. It was incredibly easy to set up my project layouts and pages.



### Automated Deployment with GitHub Actions 🤖

A modern project needs a modern workflow. I didn't want to manually build and upload my site every time I fixed a typo.

I set up a **GitHub Actions CI/CD pipeline** to handle this automatically. Here’s how it works:
1.  I `git push` my changes to the `main` branch on GitHub.
2.  A GitHub Action workflow automatically spins up a runner.
3.  The runner installs my dependencies (`npm install`).
4.  It builds the production-ready static site (`npm run build`).
5.  Finally, it deploys the contents of the `dist/` folder to my host (like GitHub Pages, Netlify, or Vercel).

This "push-to-deploy" system is incredibly efficient and lets me focus on writing code and content, not on the deployment process.



---

### What I Learned

Building this portfolio was a fantastic learning experience. It solidified my understanding of static-site generation, the power of type safety, and the convenience of a good CI/CD pipeline. Astro has quickly become one of my favorite tools for building content-heavy websites.

Thanks for reading! Feel free to [check out the source code on GitHub](https://github.com/Ron-Alex/Ron-Alex.github.io).

#### AI Generated