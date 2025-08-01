title: "Cormat Consulting"
description: "Materials Engineering & Consulting Services"
baseurl: "" 
url: "https://cormatconsulting.github.io"
theme: minimal-mistakes-jekyll
plugins:
  - jekyll-feed
  - jekyll-seo-tag
Scroll down → Commit new file.

Wait 1–3 minutes, then refresh your website.

Would you like me to prepare a full _config.yml template (multi-page menu, site name, consulting tagline) that you can just copy-paste into this new file to instantly rebuild your site?








You said:
it doesnt have anything in regard to layout


ChatGPT said:
Correct – the basic _config.yml you just recreated only has minimal info. The layout and navigation for your site are handled by:

The theme you set in _config.yml (Minimal Mistakes)

Your page files (.md or .html) which specify their layout

Navigation settings (_data/navigation.yml) for the site menu

If _config.yml was deleted, you lost the default full configuration that came with the starter template. That’s why you’re not seeing layout options now.

✅ Fix: Recreate a Proper _config.yml with Layout Options
Paste this more complete version instead of the minimal one:

yaml
Copy
Edit
title: "Cormat Consulting"
description: "Materials Engineering & Consulting Services"
baseurl: "" 
url: "https://cormatconsulting.github.io"
theme: minimal-mistakes-jekyll

# Theme settings
locale: "en-US"
logo: "/assets/images/logo.png"
author:
  name: "Cormat Consulting"
  email: "your@email.com"
  bio: "Specializing in Metallurgical Failure Analysis and Process Optimization"

# Enable minimal mistakes skins (color schemes)
minimal_mistakes_skin: "default" # options: default, dark, contrast, mint, air, neon

# Plugins
plugins:
  - jekyll-feed
  - jekyll-seo-tag
  - jekyll-sitemap

# Defaults for page layout
defaults:
  - scope:
      path: ""
      type: "pages"
    values:
      layout: "single"
      author_profile: true
  - scope:
      path: ""
      type: "posts"
    values:
      layout: "single"
      author_profile: true
      read_time: true

# Social links (optional)
social:
  linkedin: "https://linkedin.com/in/yourprofile"
  github: "https://github.com/cormatconsulting"

# Build settings
markdown: kramdown
highlighter: rouge
