# 🎨 GitHub Profile Customization Guide

Welcome to your personal GitHub profile starter pack! This guide will help you customize your profile to make it uniquely yours.

## 📝 Quick Start

Your profile README.md is already set up with a comprehensive template. Follow these steps to personalize it:

### 1. Update Basic Information

Replace the placeholder text in the header:
- `[Your Name]` - Your full name or preferred name
- `[Your Role/Title]` - e.g., "Full Stack Developer", "Data Scientist", "DevOps Engineer"
- `[Your Location]` - Your city/country or "Worldwide"

### 2. Personalize the About Me Section

Update each bullet point with your information:
- **Currently working on**: Your main project or job
- **Currently learning**: Technologies or skills you're studying
- **Looking to collaborate on**: Types of projects you're interested in
- **Ask me about**: Your areas of expertise
- **How to reach me**: Your email address
- **Fun fact**: Something interesting about you

### 3. Add Your Social Media Links

Replace `yourusername` or `youruserid` with your actual usernames:
- Twitter/X
- LinkedIn
- Instagram
- Dev.to
- Medium
- Stack Overflow

Remove any social media platforms you don't use by deleting the corresponding line.

### 4. Customize Languages and Tools

The template includes many popular technologies. To customize:

**To add a new technology:**
```html
<a href="https://technology-website.com" target="_blank" rel="noreferrer">
  <img src="https://icon-url.svg" alt="technology-name" width="40" height="40"/>
</a>
```

**To remove a technology:** Simply delete the entire `<a>` tag for that technology.

**Find more icons at:**
- [Devicon](https://devicons.github.io/devicon/)
- [Simple Icons](https://simpleicons.org/)
- [VectorLogo](https://www.vectorlogo.zone/)

### 5. GitHub Stats Themes

Your stats widgets use the `radical` theme by default. To change themes, replace `theme=radical` with any of these:

- `dark`, `radical`, `merko`, `gruvbox`, `tokyonight`
- `onedark`, `cobalt`, `synthwave`, `highcontrast`
- `dracula`, `prussian`, `monokai`, `vue`, `vue-dark`
- `shades-of-purple`, `nightowl`, `buefy`, `blue-green`
- `algolia`, `great-gatsby`, `darcula`, `bear`, `solarized-dark`
- `solarized-light`, `chartreuse-dark`, `nord`, `gotham`
- `material-palenight`, `graywhite`, `vision-friendly-dark`
- `ayu-mirage`, `midnight-purple`, `calm`, `flag-india`
- `omni`, `react`, `jolly`, `maroongold`, `yeblu`
- `blueberry`, `slateorange`, `kacho_ga`, `outrun`, `ocean_dark`
- `city_lights`, `github_dark`, `discord_old_blurple`, `aura_dark`
- `panda`, `noctis_minimus`, `cobalt2`, `swift`, `aura`
- `apprentice`, `moltack`, `codeSTACKr`, `rose_pine`

### 6. Featured Projects

Update the featured projects section with your actual repositories:
```html
<a href="https://github.com/michaelfeb/your-repo-name">
  <img src="https://github-readme-stats.vercel.app/api/pin/?username=michaelfeb&repo=your-repo-name&theme=radical" alt="Project Name" />
</a>
```

Replace `your-repo-name` with the names of your best repositories.

### 7. Set Up Blog Post Automation (Optional)

To automatically show your latest blog posts:

1. Create a `.github/workflows` directory in your repository
2. Add this workflow file `.github/workflows/blog-post-workflow.yml`:

```yaml
name: Latest blog post workflow
on:
  schedule: # Run workflow automatically
    - cron: '0 * * * *' # Runs every hour
  workflow_dispatch: # Run workflow manually

jobs:
  update-readme-with-blog:
    name: Update this repo's README with latest blog posts
    runs-on: ubuntu-latest
    steps:
      - name: Checkout
        uses: actions/checkout@v3
      - name: Pull in dev.to posts
        uses: gautamkrishnar/blog-post-workflow@v1
        with:
          feed_list: "https://dev.to/feed/yourusername"
```

Replace `yourusername` with your Dev.to, Medium, or RSS feed URL.

## 🎨 Advanced Customization

### Profile Views Counter Colors

Change the color parameter in the profile views badge:
- `?color=0e75b6` (blue)
- `?color=green`
- `?color=red`
- `?color=yellow`
- Or any hex color: `?color=ff6347`

### Stats Card Options

Add these parameters to your stats URLs:

**Hide specific stats:**
```
&hide=stars,commits,prs,issues,contribs
```

**Show icons:**
```
&show_icons=true
```

**Include private contributions:**
```
&count_private=true
```

**Custom title:**
```
&custom_title=My+GitHub+Stats
```

### Streak Stats Options

Customize your streak card:
```
?user=michaelfeb&theme=radical&hide_border=true&date_format=M%20j%5B%2C%20Y%5D
```

### Top Languages Card Layout

Change the layout:
- `&layout=compact` (default)
- `&layout=donut`
- `&layout=donut-vertical`
- `&layout=pie`

## 📚 Additional Resources

- [GitHub Profile README Generator](https://github.com/rahuldkjain/github-profile-readme-generator)
- [Awesome GitHub Profile README](https://github.com/abhisheknaiidu/awesome-github-profile-readme)
- [GitHub Readme Stats](https://github.com/anuraghazra/github-readme-stats)
- [GitHub Readme Streak Stats](https://github.com/DenverCoder1/github-readme-streak-stats)
- [GitHub Profile Trophy](https://github.com/ryo-ma/github-profile-trophy)
- [Shields.io](https://shields.io/) - Create custom badges

## 💡 Tips

1. **Keep it updated**: Regularly update your profile with new projects and skills
2. **Be authentic**: Let your personality shine through
3. **Use emojis wisely**: They add visual interest but don't overdo it
4. **Test your links**: Make sure all your social media links work
5. **Mobile-friendly**: Check how your profile looks on mobile devices
6. **Performance**: Too many dynamic widgets can slow loading times
7. **Privacy**: Don't share sensitive information

## 🔧 Troubleshooting

**Stats not showing?**
- Wait a few minutes for the API to update
- Check that your username is correct
- Ensure your repositories are public

**Images not loading?**
- Verify the image URLs are correct
- Check if the service is operational
- Try a different CDN or hosting service

**Layout looks broken?**
- Validate your HTML syntax
- Check for unclosed tags
- Preview your README in a markdown editor

## 🎉 You're All Set!

Now go ahead and make this profile your own! Don't forget to:
- ⭐ Star repositories you find helpful
- 🔄 Keep your profile updated
- 🤝 Engage with the community
- 🚀 Showcase your best work

Happy coding! 🎨
