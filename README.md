# Nuxtlific (GraphQL)

![Nuxt.js](https://img.shields.io/badge/nuxt-2.9.2-brightgreen) ![Node Version](https://img.shields.io/badge/node-v11.6.0-brightgreen) ![NPM Version](https://img.shields.io/badge/npm-6.9.0-brightgreen) [![Netlify Status](https://api.netlify.com/api/v1/badges/00905143-4df8-4d02-b65b-0a6f97ba4e85/deploy-status)](https://app.netlify.com/sites/nuxtlific/deploys) 

> **A JAM-stack framework that's so easy to use, you'll want to slap your grandma _(fucking don't though)._**

## Overview
At a high-level, [Nuxtlific](https://github.com/egstad/nuxtlific) is a blend of [Nuxt.js](https://nuxtjs.org/), [Netlify](https://www.netlify.com/docs/), and [Prismic](https://prismic.io/docs/javascript/getting-started/integrating-with-an-existing-javascript-project). Nuxt consumes data from Prismic and handles the static-generation of the app. Once pushed to github, Netlify (or a similar service) will continuously deploy the site. It's easy to learn, safe to use, and in most cases it's free. Fucking free!

This particular slice of Nuxtlific uses [GraphQL](https://graphql.org/learn/) to query Prismic instead of their default rest API. At the time of this writing (Oct. 2019), Prismic's GraphQL feature is in beta but is shipping on all new Prismic repos.

GraphQL pros:

- Dictating exactly what they need from Prismic means cleaner code and smaller file sizes.
- Retrieving many resources in a single request is easssssy.
- GraphQL is strongly-typed, letting you know what' info is available and what shape it's in.

GraphQL cons:

- Queries always return a HTTP status code of 200. This makes error handling a little tricky.
- No built-in caching support. Nuxt being a static site, this isn't a problem. But worth mentioning.
- Complexity. GraphQL comes with a learning curve, but in many cases is worth it.

GraphQL not feel like a good fit? Cool. Try out the regular version of [Nuxtlific](https://github.com/egstad/nuxtlific). It'll do ze trick.


## Installation
If you don't already have Prismic or Netlify accounts setup, start there. Both are free and won't take long. Once that is squared away, clone the repo and run the following scripts:

| Command            | Description                            |
|--------------------|----------------------------------------|
| `npm install`      | Install dependencies                   |
| `npm start`        | Launch dev server                      |

## [Wiki: A-How-Dafuq-Guide](https://github.com/egstad/nuxtlific/wiki/)

The documentaion is light, no-nonsense, and easy to read. If something is missing, let me know. Thanks babe.

## Credit

The sucker who spent some of his nights and weekends putting this shit together is Jordan Egstad. He's a graphic designer and developer living in Portland, OR. 
