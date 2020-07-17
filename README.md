
# Quick start guide for Nuxt Js

## Create new project
Need to install node(+npm,npx)

Need to install nuxt
```
  npm install --save nuxt
```

#### To create Nuxt Project
```
  npx create-nuxt-app new
```


#### Run on local machine
```
npm run dev
```

#### Run as Static website (Github pages, Nginx etc)
Update `nuxt.config.js`

```
export default {
  ...
  target: 'static',
  ...
```

Generate static files under `dist` folder
``` 
npm run build
nuxt export
```
To run Locally
```
nuxt serve
```

Content of `dist` folder can be copied to Nginx or Github pages. You can try this with Nginx docker
Replace your path to dist folder.

```
docker run -p 80:80  -v /home/abhi/github/nuxt-quickstart/new/dist:/usr/share/nginx/html:ro nginx
```
## To run this 

``` 
git clone
cd 
npm install
```

## Demo Site
https://akumar261089.github.io/nuxtjs-quickstart/