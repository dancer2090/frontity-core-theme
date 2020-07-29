# Sirinsoftware

Sirinsoftware uses Frontity for connecting with Wordpress admin.

## Installation

Use the `npm` or `yarn` package manager to install project.

```bash
cd sirinsoftware
npm install
or
yarn install
```

## Installation package

Use the `npm` or `yarn` package manager to install project.

```bash
cd project-folder
npm install @analytics/google-tag-manager @frontity/core @frontity/head-tags @frontity/html2react @frontity/mars-theme @frontity/tiny-router @frontity/wp-source analytics axios dotenv frontity react-google-recaptcha-v3 react-modal react-resize-detector eact-id-swiper react-spinners

and
npm install --save-dev eslint eslint-config-airbnb eslint-plugin-import eslint-plugin-jsx-a11y eslint-plugin-react eslint-plugin-react-hooks

or
yarn add @analytics/google-tag-manager @frontity/core @frontity/head-tags @frontity/html2react @frontity/mars-theme @frontity/tiny-router @frontity/wp-source analytics axios dotenv frontity react-google-recaptcha-v3 react-modal react-resize-detector eact-id-swiper react-spinners

and

yarn add --dev eslint eslint-config-airbnb eslint-plugin-import eslint-plugin-jsx-a11y eslint-plugin-react eslint-plugin-react-hooks
```

## Usage

Recommended `node.js` version - `12.16.3`

### Development

In `frontity.settings.js` set the Wordpress API URL: 
```javascript
{
   "name": "@frontity/wp-source",
   "state": {
      "source": {
        "api": "https://admin.sirinsoftware.com/wp-json"
      }
   }
},
```

#### Local running

```bash
npm run dev
or
npx frontity dev --port YOUR_PORT
```
#### Production build

```bash 
npm run build
```

#### Production server test

```bash 
npm run serve
```
Sometimes `serve` command returns error. If you get it, run 
```bash 
node index.js
```

### Deployment strategy

The `master` branch deploys every 2 days.
To add the code to master:
1. Create another branch from master. ( follow names `featute/branchmane` or `fix/branchname`)
2. Create PR. Assign someone to check it.
3. After approvement code merges to master.


### Deployment (server)

1. Install  `node.js` version - `12.16.3`
2. Run the progect
```bash
npm intsall
npm run build
npm run serve
``` 
Sometimes `serve` command returns error. If you get it, run 
```bash 
node index.js
```

Optional you can use PM2 for restarting application.


