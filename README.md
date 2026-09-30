# rocksteady-fitness-redirect

Redirects the old domain **rocksteady-fitness.com** to **[rocksteadyfitness.com](https://rocksteadyfitness.com)**,
keeping the path (so `/pages/privacy.html` lands on the new privacy page).

The real site lives in [rocksteady-fitness-website](https://github.com/SeanCrotty/rocksteady-fitness-website).

- `CNAME` claims the old domain for GitHub Pages.
- `index.html` and `404.html` are identical: `404.html` handles every path that doesn't exist in this repo,
  which is all of them.
- The redirect is JavaScript (`location.replace`), with a meta refresh to the homepage as a fallback.

Keep this repo and the old domain registered — the live App Store listing and older app builds link to it.
