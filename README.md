# Boys Middle School Website

A modern Astro website for the boys middle school project.

## Development

```bash
npm install
npm run dev
```

## Build

```bash
npm run build
```

### Deploy
```
aws s3 sync dist/ s3://boysms-org-site-origin/ --delete --profile YOUR_PROFILE

aws cloudfront create-invalidation \
  --distribution-id E3IRF34YS8TJNX \
  --paths "/*" \
  --profile YOUR_PROFILE
```

