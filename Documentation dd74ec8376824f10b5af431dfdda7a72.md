# Documentation

[Datasource Onboarding](Datasource%20Onboarding%206842921f039944f8a4cd5f618ccccf40.md)

[User Management](User%20Management%204cec064a73e14a619d3eaf694de7f698.md)

[Project Builder](Project%20Builder%207d59ea7b603648dfb0c80430255b2e2b.md)

[Embedding Documentation](Embedding%20Documentation%2050702aa0ad7e46cc8da8390e461e79fd.md)

# Documentation

> Aether is perfect for building out documentation of all kinds, check out the content below for examples on what can be achieved.
> 

<aside>
⚡ [Check out the official Super documentation built using Aether here](https://docs.super.so)

</aside>

## Code Documentation

### Environment Variables

Aether has built-in support for loading environment variables into the browser and Functions. Loading environment variables into Node.js requires a small code snippet. In development, Aether will load environment variables from a file named `.env.development`. For builds, it will load from `.env.production`.

A `.env` file could look like:

```
Aether=https://dev.example.com/apiAPI_KEY=927349872349798
```

To load these into Node.js, add the following code snippet to the top of your `Aether-config.js` file:

```jsx
require("dotenv").config({  path: `.env.${process.env.NODE_ENV}`,})
```

This loads `process.env.AETHER_API_URL` and `process.env.API_KEY` for use in `Aether-*.js` files and functions.

For example, when configuring a plugin in `aether-config.js`:

```jsx
require("dotenv").config({  
	path: `.env.${process.env.NODE_ENV}`,
})

module.exports = {  
	plugins: [    
		{      
			resolve: `aether`,      
			options: {        
				apiKey: process.env.API_KEY,      
			},    
		},  
	],
}
```

### **Accessing Environment Variables in the browser.**

By default, environment variables are only available in Node.js code and are not available in the browser as some variables should be kept secret and not exposed to anyone visiting the site.

To expose a variable in the browser, you must preface its name with `AETHER_`. So `AETHER_API_URL` will be available in browser code but `API_KEY` will not.

Variables are set when JavaScript is compiled so when the development server is started or you build your site.

```jsx
import React, { useState, useEffect } from "react"
function App() {
  const [data, setData] = useState()
  useEffect(async () => {
    const result = await fetch(
      `${process.env.AETHER_API_URL}/users`
    ).then(res => res.json())
    setData(result.data)
  })
  return (
    <ul>
      {data.map(user => (
        <li key={user.id}>
          <a href={user.url}>{user.name}</a>
        </li>
      ))}
    </ul>
  )
}
export default App
```

### **Add `.env*` files to .gitignore**

Environment variable files should not be committed to Git as they often contain secrets which are not safe to add to Git. Instead, add `.env.*` to your `.gitignore` file and setup the environment variables manually locally.

---

## Reference Tables

### Light mode colors

[Light Mode](Documentation%20dd74ec8376824f10b5af431dfdda7a72/Light%20Mode%20ce0328aa93644664a0c62760998ab255.csv)

### Dark mode colors

[Dark Mode](Documentation%20dd74ec8376824f10b5af431dfdda7a72/Dark%20Mode%20159874397f4747268edcd4bac0e6d787.csv)

---

## Guides and Instructions

### Adding a custom domain to your site

To add a domain to your site, first head into your site editor (cog icon) and click into the **"Domains"** page, then click the **"Add a custom domain"** button. After entering your own domain address in the popup, you'll then need to make some changes to the DNS settings through your hosting provider.

You would need to do this through your domain registrar's (GoDaddy, Namecheap, Google Domains, etc) or DNS provider's (Cloudflare, Netlify, etc) website. For specific instructions, view the content inside the toggle blocks below.

## DNS Settings

Below you can find the DNS settings that need to be included on your domain registrar's (GoDaddy, Namecheap, Google Domains, etc) or DNS provider's (Cloudflare, Netlify, etc) website.

### Root domain records

For a root domain like `example.com` you'll need to add the following records:

[      ](Documentation%20dd74ec8376824f10b5af431dfdda7a72/Untitled%2064823630429143e381f8b9a2378a0707.csv)

### Subdomain records

For a subdomain like `blog.example.com` add this record:

[     ](Documentation%20dd74ec8376824f10b5af431dfdda7a72/Untitled%20b10f1960dbe14fb28c2c0e50e8df1ff9.csv)

**If you run into issues, please make sure that you have:**

- Added new DNS records to your domain provider
- Removed old DNS records
- Waited up to 24 hours for new settings to propagate

<aside>
💡 This tool can be used to check if the records are set up correctly: [https://www.whatsmydns.net/](https://www.whatsmydns.net/)

</aside>

← Previous

[Blocks](Project%20Builder%207d59ea7b603648dfb0c80430255b2e2b.md)

Next →

[Design System](Embedding%20Documentation%2050702aa0ad7e46cc8da8390e461e79fd.md)

On this page