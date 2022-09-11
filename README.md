# Basic Elm + Tailwind project scaffold

### About

This is about the bare minimum project setup for an Elm frontend with Tailwindcss

If you deploy to production, you're going to need to alter the `<link>` tag in `index.html` to point somewhere other than the current directory for `dist.css`. 

To get your tailwind classes to update:
`npx tailwindcss -i app.css -o dist.css`

If you're using Vim, create or add the `makeprg` from [my elm.vim](https://gist.github.com/JohnnyCurran/1ec9d62171ab6d55eec07b9e7c2118e0) to use `:make` (or `:Make`) if you're using `Dispatch.vim` for background builds

Then, when you make you compile your elm files, the tailwind utility classes get picked up and put into dist.css. Just refresh `index.html` and see your changes come to life :)
