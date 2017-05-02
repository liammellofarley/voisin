# Documentation
Everything you can tweak is in the _EDIT folders.

In those folders are files that end in .md this stands for markdown

Each .md file corresponds to a specific post, everything should be named in a way that makes sense so you can tell what connects to what.

To add new posts for the timeline or new partners, copy one of the existing ones or create a new appropriately named file ending in .md and then mimick the structure of an existing post.

Each .md file is made of two parts: frontmatter and body.

# Front Matter

The front matter is the variables that define each post. It comes between the two "---" These are as follows:

Title: The title of each post, the bold text at the top.

Weight: Determines the order in which it's placed.

Img: Used exclusively for farmers. The images should be placed in the /images/partners folder then for the variable you give the image name including the .jpg. Please name all the images things that make sense and don't use spaces.

Class: Places partners in the category they belong, possible options are farmer, gund, ufsc.

# Body

The body is written in a language called markdown, it comes after the final "--". For 99% of stuff that means you just type text in, but there are some places where you may want to make headers (bold and larger font), bold or italicize, or put links and images in. 

Images are the one thing that's specific to this site so here's how to do them:

```markdown
!["Description"]({{ site.url }}/images/"imagepath.jpg")
```
Just replace what's in quotes with your description and the filename of your image.
eg:
```markdown
![Standin for profile pictures]({{ site.url }}/images/profile-standin.jpg)
```
How it'll look
![Standin for profile pictures](https://liammellofarley.github.io/voisin//images/profile-standin.jpg)


For pretty much anything else including adding images that are not hosted on the site check out this link that explains how to use markdown https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
