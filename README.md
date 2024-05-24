# Minimalism

<a href="https://11ty-minimalism.netlify.app/" target="blank_">
   <img alt="antreprima" src="http://marcomicale.altervista.org/minimalism.webp" width="100%" >
</a>

> Simplicity is the ultimate sophistication!

## What do I want to get?

- ✅ Quick page creation
- ✅ Customizable Favicon (msapplication/apple/safari/chrome)
- ✅ Blog
- ✅ Fedd Rss
- ✅ Sitemap
- ✅ PWA
- ✅ Dynamic social images for each page/post
- ✅ SEO optimization
- ✅ 404 error page
- ✅ Offline page
- ✅ Easy social links - edit /src/_11ty/_data/meta.js
- ✅ All 100 in lighthouse
- ✅ Light/Dark mode
- ✅ [Netifly](https://www.netlify.com/)

## What I used:

- [Eleventy](https://github.com/11ty/eleventy)
   - [Plugin eleventy-img](https://github.com/11ty/eleventy-img)
   - [Plugin eleventy-plugin-rss](https://github.com/11ty/eleventy-plugin-rss)
   - [Plugin eleventy-navigation](https://github.com/11ty/eleventy-navigation)
   - [Plugin-social-images](https://github.com/5t3ph/eleventy-plugin-social-images)
   - [Plugin-reading-time](https://github.com/johanbrook/eleventy-plugin-reading-time)
- [Tailwindcss](https://github.com/tailwindlabs/tailwindcss)
   - [Tailwindcss typography](https://github.com/tailwindlabs/tailwindcss-typography)
- [Slugify]([https://github.com/simov/slugify)
- [Luxon](https://github.com/moment/luxon)
- [html minifier](https://github.com/kangax/html-minifier)
- [rimraf](https://github.com/isaacs/rimraf)
- [npm-run-all](https://github.com/mysticatea/npm-run-all)
- [Tabler Icon](https://github.com/tabler/tabler-icons)

## Status
### BETA

Usable but with some corrections to be made.

## Folder Tree

```bash
Minimalism
|    .eleventy.js
|    .gitattributes
|    .gitignore
|    LICENSE
|    logo.png # Replace this file with your logo
|    netlify.toml
|    package-lock.json
|    package.json
|    README.md
|    SECURITY.md
|    tailwind.config.js
|
+---.github
|    \---workflows
|            codeql-analysis.yml
|
+---.vscode
|        tasks.json
|
\---src
     |    ... # Add the pages you want
     |    blog.md # Your blog page (edit the intro from here)
     |    index.md # The front page of your site (essential)
     |
     +---blog
     |        ... # Enter your blog posts here
     |
     \---_11ty
         +---_date
         |        meta.js # EDIT THIS FILE!
         |
         +---_generate
         |        404.njk
         |        feed.njk
         |        manifest.njk
         |        offline.njk # Page shown by the app if offline
         |        pagesjson.njk
         |        robot.njk
         |        sitemap.njk
         |        socialtemplate.njk # Edit if you want to change the social image
         |
         +---_includes
         |        favicon.njk
         |        footer.njk
         |        head-article.njk
         |        head-website.njk
         |        head.njk
         |        nav.njk # Site Header (Title and Nav Bar)
         |
         +---_layouts # Layouts:
         |        article.njk # Blog Articles
         |        blog.njk # Blog Page
         |        page.njk # Generic pages
         |
         +---_social # Files generated for the social image
         |        pages.json
         |        social.css
         |        template.html
         |
         +---_static
         |    +---app # Static resources
         |    |        .htaccess
         |    |        sw.js
         |    |
         |    +---favicon
         |    |        ... # Favicon Generate from the logo.png file
         |    |
         |    \---img
         |            ...
         |
         \---_tailwindCSS
                 raw-social.css # CSS of your site
                 raw-website.css # Edit if you want to change the social image
```
