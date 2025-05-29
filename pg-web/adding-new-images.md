# 🖼 Adding New Images to the Hugo Site

This guide explains where to put new images for your site and how to reference them.

---

## ✅ Site-wide images

For general images used across the site (e.g., logos, banners, shared assets),  
place them in:

`static/images/`


### Example usage in Markdown:
```markdown
![Alt Text](/images/my-picture.jpg)
```
The /images/my-picture.jpg path refers to /static/images/my-picture.jpg.

Files under static/ are served as-is at the site root.

✅ Post-specific images

If you want images tightly linked to a specific post,
place them in a folder next to the post file:

`content/posts/my-post/`

Example:

```
content/posts/my-post/index.md
content/posts/my-post/image1.jpg
```

Usage inside the post:
```markdown
![Alt Text](image1.jpg)
```

✅ Note:

Hugo automatically links relative image paths when they are in the same folder as the post.

⚠ Important
1. Keep image filenames clean and lowercase (avoid spaces).
2. Optimize large images before uploading to reduce site size.
3. For background or theme images, check if the theme uses assets from static/.

