# How to deploy a next js application to Netlify using the command line?

- At first, you have to install netlify-cli globaly
```
npm install -g netlify-cli
```
- Then you have to log in to your netlify account
```
  ntl login
```
- Install this package to your next js application
```
npm i -D @netlify/plugin-nextjs
```
- Then create a file named `netlify.toml` in your project root
- Put this code on this file
```
[[plugins]]
package = "@netlify/plugin-nextjs"

[build]
command = "yarn next build"
publish = ".next"
```

- Then run
```
netlify deploy --build --prod
```
- And provide the necessary information
![Netlify Deploy Image](https://i.ibb.co/TrN2GnP/netlify-deploy.png)

- Wow! Wow! and Wow finally you deployed your next JS application to Netlify
![Netlify Deploy Completed Image](https://i.ibb.co/Tk6tKny/deploy-completed.png)
