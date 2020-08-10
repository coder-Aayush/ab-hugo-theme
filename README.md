### How to Use this theme

Create Hugo Project

```
Hugo new site <project name>
```

Make sure you have hugo install. For installing hugo check [Hugo Documentation](https://gohugo.io/getting-started/installing#readout)

At the root of your Hugo project, run:

```
git submodule add https://github.com/coder-Aayush/ab-hugo-theme themes/ab-hugo-theme
```

Add **AB HUGO Theme** at you _config.tomol_ file.

```
theme = "ab-hugo-theme"
```

Next, copy the contents of the [config.tomol](exampleSite/config.tomol) to your site's config.toml. Make sure to read all the comments.

Finally, Run

```
hugo server -D
```

**Note: If you are seeing a blank page it is probably because you have nothing in your content/ directory. Read on to fix that.**

###Configuring the Home Page
In the **config.tomol** file you can customize homepage.

```
title = "Title of Your Website"
```

You can always override all the template in **layouts folder**

### Confugring Paramaters

This paramaters are all over the site. If you don't like confuging just copy & paste as same.

```
[params]
  bio = "I am Hugo Coder"
  discription = "Hola I am aayush"
  author = "Aayush Bhattarai"
  showcredit = true
  favicon = "/img/ab-hugo-coder.ico"
  featuredImage = "" # add Featured Image inside /assets/images and your path be like /images/filename.jpg
  disqusShortname = "" # get username from disqus
  showComment = true # either true or false
```

**Note Add your Images inside _/assets/images_ and path must be _/images/filename.jpg_\* Must contain "/" at front of filename**

### Social Icons

In your _config.tomol_ file add

```
[[params.social]]
        url   = "https://twitter.com/"
        icon  = "twitter"
    [[params.social]]
        url   = "https://facebook.com/"
        icon  = "facebook-f"
    [[params.social]]
        url = "mailto:youremail@email.com"  # For a direct email link, use "mailto:test@example.org".
        icon = "paper-plane"
```

**Note: Use Icon From [Font Awesome](https://fontawesome.com/v4.7.0/icons/)**

### Creating Blog Post

You can create a new blog post page by going to the root of your project and typing:

```
hugo new posts/<my-lifestyle-post>.md
```

**Note: You Must Type _Posts_ and Your FileName. If You don't do so, then Your Post is not Visiable**

Now Open **content/posts<my-lifestyle-post>.md file and start writing post. [Learn markdown Here](https://guides.github.com/features/mastering-markdown/)**

### Creating About Page and Other Pages

You can simply create about page using this command.

```
hugo new about.md
```

**Note: Here you shouldn't write _posts_ path. You can also add other file just using this command.**

Example

```
hugo new gallery.md
```

### Displaying Other Pages in Menu/Nav

For Displaying Your other files like _gallery.md_, Open _config.tomol file and type_

```
[[menu.main]]
name = "Gallery"
url = "/gallery/"
# add  more same like this...

[[menu.main]]
name = "About"
url = "/about/"

[[menu.main]]
name = "GitHub"
url = "https://github.com/coder-Aayush"
```

### Adding Favicon

Add you favicon at _static/img_ also yo need to add in _config.tomol_ file

```hugo
[params]
  ....
  favicon = "/img/ab-hugo-coder.ico" #must start with "/"
  ....
```

You can also Add Featured Image same as above.
This is the confugration for **AB Hugo Theme.** For more you can see [config.tomol](https://github.com/coder-Aayush/ab-hugo-theme/blob/)
