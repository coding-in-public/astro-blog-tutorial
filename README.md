# Moving to the 2.0 Content Collections API

Video link: https://youtu.be/zUmqmuSvJMs

In this video, I’ll take you through the process of updating our blog to the new Content Collections API for a type-safe markdown experience with error-checking that actually helps!

## General steps we’ll cover
1. Update all packages to the latest versions (if you’re viewing this well into the future, you may want to update to the specific versions in the repo)
`npx ncu -u`
2. Update tsconfig.json and add .astro to .gitignore
3. Create content/config.ts and define the blog collection
4. Move all posts to /content/blog/
5. Change “frontmatter” to “data” site-wide and change “url” to “slug” site-wide
6. Switch out all .glob() imports to use the getCollection method from astro:content
7. Ensure all links point to `/blog/[slug]/`
8. Move old BlogPostLayout to /blog/ directory and update code inside of a getStaticPaths function
9. Update RSS to use getCollection method

## Links

👨‍🚀 Astro Course Links 👨‍🚀
- Github final: https://github.com/coding-in-public/astro-blog-tutorial/tree/content-collections-api
- Demo site: https://codinginpublic.dev/projects/astro-blog-tutorial/
- Full Astro Blog Course playlist: https://youtube.com/playlist?list=PLoqZcxvpWzzeRwF8TEpXHtO7KYY6cNJeF

---------------------------------------

🔗  Key Links 🔗
- Content Collections Docs: https://docs.astro.build/en/guides/content-collections/
- Zod docs: https://zod.dev/

---------------------------------------

🔗  Additional Links 🔗
- My clipboard: Pastebot (https://tapbots.com/pastebot/)
- My terminal: Warp (https://www.youtube.com/watch?v=wdrjIHzGW74)
- Autocomplete in VSCode: fig.io

---------------------------------------

📹  Related Videos 📹
- Playlist for Astro series: https://youtube.com/playlist?list=PLoqZcxvpWzzeRwF8TEpXHtO7KYY6cNJeF


---------------------------------------
🎨 VSCode Theming
- Font: Cascadia Code: https://github.com/microsoft/cascadia-code
- Theme: https://marketplace.visualstudio.com/items?itemName=Equinusocio.vsc-community-material-theme
- Icons: https://marketplace.visualstudio.com/items?itemName=BeardedBear.beardedicons

---------------------------------------

🌐 Connect With Me 🌐
- Website: https://codinginpublic.dev
- Blog: https://chrispennington.blog
- Twitter: https://twitter.com/cpenned
- Patreon: https://www.patreon.com/coding_in_public
- Buy Me a Coffee: https://www.buymeacoffee.com/chrispennington