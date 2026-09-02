# MyBDResults24 Education Board Result Backend

Cloudflare Pages Functions backend for the Blogger result checker.

## Deploy
1. Upload this repository to GitHub.
2. Create a Cloudflare Pages project from the repository.
3. Add secret environment variable `API_SECRET` with a long random value.
4. Deploy.
5. Test `https://YOUR-PAGES-DOMAIN/api/health`.
6. Put the Pages URL into the Blogger HTML `API_BASE` variable.

The backend uses the official educationboardresults.gov.bd workflow and does not solve or bypass CAPTCHA; the visitor enters the CAPTCHA displayed by the official service.

If the government portal changes its endpoint or field names, update only `functions/api/result.ts` and/or `functions/api/captcha.ts`.
