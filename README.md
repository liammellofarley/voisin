# Documentation
Everything you can tweak is in the _EDIT folders.

In those folders are files that end in .md this stands for markdown

Each .md file corresponds to a specific post, everything should be named in a way that makes sense so you can tell what connects to what.

To add new posts for the timeline or new partners create a new file in the relevant folder and name it appropriately eg:"joshuafarley.md" in the /partners/gund folder. Next open an existing .md from the same folder and click "raw". Copy everything from that file then go back to your file and paste it in. The button to edit files is a little pencil, you can alternatively use that and copy the contents from their when you're copying other .mds as well.If you feel 100% comfortable with how the files are structured feel free to type up the frontmatter from memory.

Each .md file is made of two parts: frontmatter and body.

## Front Matter

The front matter is the variables that define each post. It comes between the two "---" These are as follows:

### Common Variables
title: The title of each post, the bold text at the top.

weight: Determines the order in which it's placed. Smaller numbers first.

img: Used exclusively for farmers. The images should be placed in the /images/partners folder then for the variable you give the image name including the .jpg. Images should be 256x256 and ideally just a headshot, I'll have some examples up soon. Please name all the images things that make sense and don't use spaces.

class: Places partners in the category they belong, possible options are farmer, gund, ufsc.

type: You shouldn't have to mess with this. It attaches a description to the correct category.

### Timeline

Due to Emmajane's request that the timeline go in reverse chronological order there are some abnormalities here.

#### Variables present in all timeline elements

title: Title of each timeline element

weight: Determines the order of elements with bigger numbers first. Since the Phases are in reverse chronological order but the elements within a phase are in chronological order we use x.x convention, where 1.9 is the first post in phase 1, so it shows up under the other phases but above the other elements in phase 1.

time: Vestigial variable, currently does nothing.

#### Variables present in elements that mark a new phase

phase: This both indicates that this element marks a new phase and names the phase numerically. This must follow a Phase # convention eg: Phase 1.

phase-time: This changes the date next to the phase name eg: 1998-2000.

direction: This will flip the side the phase and the phase-time are displayed on. If the phase text appears on the right add left to this variable eg: direction: left, if the phase is on the right and this variable is set to left simply clear it. This can be used to align all the phase labels on one side of the page. It's a small hack that simplifies a lot of the code but this is the resulting inconvenience.

### Research

Research has no special variables but I'm mentioning it here because uses only one .md file per category. Simply put a line between different posts within categories here.

## Body

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

For videos (assuming youtube), simply click embed under the video on youtube and copy the html. Markdown supports inline html so it will work perfectly.

For pretty much anything else including adding images that are not hosted on the site check out this link that explains how to use markdown https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet

# Updating the site

You don't have to do anything but save/commit changes when you're done editing and then the site should automatically update within a couple of minutes. If anything goes wrong github has backups of every single commit so you can roll back. So if you mess up contact me and I can roll it back.
