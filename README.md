# How to deploy a next js application to netlify using comand line

- At first have to install netlify-cli globaly `npm install -g netlify-cli`
- Then you have to log in to your netlify account `ntl login`
- Install this package to your next js application `npm i -D @netlify/plugin-nextjs`
- Then create a file named **netlify.toml** in your project root
- Put this code on this file
```
[[plugins]]
package = "@netlify/plugin-nextjs"

[build]
command = "yarn next build"
publish = ".next"
```

- Then run `netlify deploy --build --prod` and provide the necessary informations
