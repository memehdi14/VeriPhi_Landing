# How to Get Your Live URL (Hackathon Submission)

You need a live link for the landing page to submit. The extension itself lives on GitHub, but this page sells it.

## Option 1: Vercel (Recommended - Professional)
1. Open your terminal in VS Code.
2. Run:
   ```powershell
   cd "c:\MMD Public\Hackathons\Techsprint\landing-page"
   npx vercel
   ```
3. Follow the prompts:
   - Sets up and deploys? [Y]
   - Which scope? [Enter]
   - Link to existing project? [N]
   - Project name? [Enter] (e.g., veriphi-landing)
   - Directory? [Enter] (default is `.`)
4. **Done!** It will give you a `Production: https://veriphi-landing.vercel.app` link. Use this for submission.

## Option 2: Netlify Drop (Fastest - No Terminal)
1. Go to the `landing-page` folder in your file explorer.
2. Run `npm run build` (I already ran this for you).
3. Locate the `dist` folder inside `landing-page`.
4. Go to [app.netlify.com/drop](https://app.netlify.com/drop).
5. Drag and drop the `dist` folder onto the page.
6. **Done!** You get a live URL immediately.

## Option 3: GitHub Pages
1. Push this `landing-page` folder to a GitHub repository.
2. Enable GitHub Pages in Settings -> Pages.
3. Choose `landing-page` directory if possible, or deploy via Actions. (Vercel is easier).
