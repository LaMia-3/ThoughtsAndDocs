# Fixing SPA Routing on Vercel

## Source
- Author: Sathish Kumar
- URL/Publication: https://medium.com/today-i-solved/deploy-spa-with-react-router-to-vercel-d10a6b2bfde8
- Date: Not specified (accessed February 16, 2026)

## Summary
This article explains how to fix the common 404 NOT_FOUND errors that occur when deploying Single Page Applications (SPAs) with client-side routing (like React Router) to Vercel. The issue happens when users directly access routes like `/collections` or `/series` instead of navigating to them from the home page.

## Key Points
- SPAs with client-side routing face 404 errors on direct URL access when deployed to Vercel
- The problem occurs because Vercel looks for physical files at the specified paths
- The solution is to create a `vercel.json` configuration file in the project root
- The configuration redirects all requests to the `index.html` file, allowing React Router to handle the routing

```json
{
  "rewrites": [
    {
      "source": "/(.*)",
      "destination": "/index.html"
    }
  ]
}
```

## Quotes
> "When you deploy a SPA with React Router to Vercel, you might encounter a 404 error when accessing routes directly. This happens because Vercel is looking for physical files at those paths."

> "To fix this issue, you need to create a vercel.json file in your project root with the following configuration."

## Personal Notes
- I've encountered this issue multiple times with both my Book Collection App and Notely projects
- The solution works consistently across different React projects using React Router
- This is a must-have configuration for any SPA deployed to Vercel
- The same issue/solution applies to other hosting platforms like Netlify (though with different configuration files)
- Remember to add this configuration before deploying to avoid routing issues

## Related References
- [React Router Documentation](https://reactrouter.com/en/main)
- [Vercel Documentation on Rewrites](https://vercel.com/docs/concepts/projects/project-configuration#rewrites)

## Tags
#reference #vercel #react #spa #routing #deployment #troubleshooting
