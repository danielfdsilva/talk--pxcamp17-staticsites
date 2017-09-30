# Preparation
- [ ] Clean the `metalsmith.js`
- [ ] Clean `_prose.yml`
- [ ] Remove `GH_REF` and `fingerprint` from `.circleci/config.yml`
- [ ] Delete uneeded posts
- [ ] Delete `.git`


# Slide 1

- Introduction
- static sites are nothing new. they've been around since ever
- Maintaining static files was a nightmare, and CMS came into play.
- I'm not going to explain how to build a static site but rather show you a set of tools and a workflow to work with static site.
- By the end of the talk we'll have, hopefully, a auto-deployable website hosted on gh-pages and that uses prose.io for content management.



# Slide 2

- Brief explanation of each tool


## Slide 2.1 - Metalsmith

- Very simple library.
- Doesn't make assumptions on how you structure your project.
- Uses plugins for all logic
- You can use Metalsmith for more things than just rendering sites. You could create an API with it for example


## Slide 2.2 - Github

- Everyone knows GH
- Free for OS
- Version control and Hosting


## Slide 2.3 - Prose

- Simple file editor geared towards md files.
- Can edit any text file


## Slide 2.4 - Circle

- Fast continuous integration service
- Free for OS projects

>> As long as you keep your source public, you can go by without spending anything.


---


# Demo

## Metalsmith

- Show structure.
- Create the metalsmith config. No need to know the config by heart, just look at the docs. Explain custom plugin.
- Anatomy of a post
- Layouts
- Render and explain build system (`pyserve 4000`)

## Prose and GH

- The prose file defines how prose reads the repo and how users edit the files.
- Create the prose file. Explain field types
- Create repo and commit
- Show prose interface
- Create new post (Mind the publish flag)
- Show changes on GH

## Circle CI
- Explain config file.
- Add key
- **Change the base url**
- Push
- Test with prose.io