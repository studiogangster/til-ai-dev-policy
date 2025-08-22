# til-ai-dev-policy

## Deploying to Cloudflare Pages

1. Install Wrangler globally if you haven't:
   ```
   npm install -g wrangler
   ```

2. Set your Cloudflare account ID in `site/wrangler.json`:
   ```
   "account_id": "YOUR_CLOUDFLARE_ACCOUNT_ID"
   ```

3. Deploy the site:
   ```
   npx wrangler pages deploy . --project-name=secure-guidelines
   ```

4. For more details, see: https://developers.cloudflare.com/pages/framework-guides/deploy-a-static-site/
