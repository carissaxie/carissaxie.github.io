# TODO — follow-ups for the website

## 1. Finish Google Search Console verification (get indexed by Google)

**Status:** the verification meta tag is already live on the site
(`<meta name="google-site-verification" content="EgfZumiO…">` in every page's `<head>`),
but clicking **Verify** in Search Console failed on the first try.

**To finish (a few minutes):**
1. Go to <https://search.google.com/search-console>.
2. Property = URL prefix **`https://carissaxie.github.io`**, method **HTML tag**.
3. Click **Verify** again. The tag is confirmed live, so a retry usually works
   (Google's fetch sometimes lags; wait a minute and retry if needed).
4. If the HTML-tag method keeps failing, use the **HTML file** method instead:
   - Search Console gives you a file like `googer abc123.html` to download.
   - Send me that file (or its name + contents) and I'll commit it to the repo root,
     then click Verify.
5. Once verified, go to **Sitemaps** in the left sidebar and submit: `sitemap.xml`.

After this, Google typically starts showing the site for name searches within a few
days to ~2 weeks.

## 2. Replace placeholder assets with real files
- `profile.jpg` (repo root) — your headshot (square works best, ~500×500+).
- `assets/cv.pdf` — your real CV. (You said you'll provide a Word doc; I can convert it
  to PDF and/or link it — just get the file onto the machine and tell me.)

## 3. Fill in real CV details
- `cv.qmd` still has placeholder Education/Experience dates and entries — update once the
  CV is finalized. Affiliation (A*STAR Genome Institute of Singapore) is already set.

## 4. (Optional) Custom domain — deferred
- Currently on the free `carissaxie.github.io`. A custom domain (e.g. `yixie.bio`) is a
  ~5-minute swap later if ever wanted; see `PLAN.md` Step 7.
