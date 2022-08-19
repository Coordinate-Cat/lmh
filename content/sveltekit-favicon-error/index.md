---
title: Issue with sveltekit returning 500 Error for favicon
date: 2022-08-19
description: Why does it return a 500 error?
isCompleted: true
emoji: 🔨
slug: sveltekit-favicon-error
tags: [svelte, sveltekit, vercel, vite]
---

# Issue
<figure>
    <img src="https://user-images.githubusercontent.com/42393004/185533680-e75d4e31-3d0a-479d-8529-721e9ae44858.png"
         alt="500(Internal Server Error)">
    <figcaption>500(Internal Server Error)</figcaption>
</figure>

I don't know when it started, but when I launch sveltekit and make a screen transition, it returns a 500 error.

I was having trouble solving the problem by switching the favicon extension to .png or .ico.
Also rewrote the svelte-specific `%svelte.assets%` to the path where the favicon is actually located, but this did not solve the problem.

However, this was easier than expected to fix with the following modification.

[Why is sveltekit fetching for favicon.png in subpath?](https://stackoverflow.com/questions/71049580/why-is-sveltekit-fetching-for-favicon-png-in-subpath)

In the comments below the question of this one, I found the following answer.
> href="%svelte.assets%/favicon.png"- I added a slash to this line and the error went away - href="/%svelte.assets%/favicon.png"

Apparently, all you need to do is prefix `%svelte.assets%` with `/`. Like this `/%svelte.assets%/favicon.ico`.