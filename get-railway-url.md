# How to Get Your Railway Backend URL

## Quick Steps:

1. **Go to Railway Dashboard**: https://railway.app/dashboard
2. **Find your backend project** (the one that contains your Node.js/Express app)
3. **Click on the project**
4. **Look for the "Deployments" tab**
5. **Find your latest deployment**
6. **Copy the URL** (it will look like: `https://your-app-name-production.up.railway.app`)

## Alternative Method:

1. **Go to your project settings**
2. **Look for "Domains" or "Custom Domains"**
3. **Copy the Railway-provided domain**

## Once you have the URL:

1. **Add `/api` to the end** (e.g., `https://your-app-name-production.up.railway.app/api`)
2. **Set this as your `VITE_API_URL` environment variable in Netlify**
3. **Update the fallback URL in `frontend/src/lib/axios.ts`**

## Test the URL:

Try visiting your Railway URL in a browser. You should see:

```
Welcome to B&W API
```

If you see this, your backend is working correctly!