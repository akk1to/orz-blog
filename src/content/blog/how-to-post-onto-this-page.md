---
title: "How to publish a post on this page"
description: "A how-to guide to publish a new post on this page"
published: "1735273160000"
author: "akk1to.dev"
heroImage: "https://images.alphacoders.com/135/1357322.jpeg"
---
*This post will show you how to publish a new post on this blog, hosted by ChuyenTin Organisation. Note that you need to make a new PR on the exact post folder to publish a new post onto this page.*
*This page was made and maintained by akk1to.dev (idea from [Willam Harrison's blog](https://blog.wharrison.com.au/))*

## 1. Generate ideas & write a new post
First, generate your ideas and write a new post using Markdown format. You can use popular Markdown editors like [StackEdit](https://stackedit.io) or [Visual Studio Code](https://code.visualstudio.com) to assist you in writing. For every post, be sure to follow the specified file format to ensure that your post is clearly displayed on the page.
```md
---
title: "(your post title goes here)"
description: "(your post description goes here)"
published: "(formatted date, see how to get it below)"
heroImage: "(banner of the post, delete this line if you want to make it random)"
---
(your post content below here)
```
Our post system uses a formatted time method, called Unix timestamp in **miliseconds**. You can use online tools to encode the date to Unix timestamp in miliseconds format such as [EpochConverter](https://epochconverter.com/) to encode it and put inside the file.
<p align="center">
    <img src="https://i.imgur.com/mpMGO1w.png"></img>
    <i>EpochConverter homepage</i>
</p>
To put image in this post, you can upload it onto imgur and stick it in the post using these methods.

```md
![image](https://i.imgur.com/mpMGO1w.png)
```
<p align="center"><i>An example using ![image] tag in markdown</i></p>

```html
<p align="center">
    <img src="https://i.imgur.com/mpMGO1w.png"></img>
</p>
```
<p align="center"><i>An example using HTML tags to center the image</i></p>

You can check out [this link](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax) to know how to write a markdown file.
Once you're ready, move to step 2 to post your blog post onto the page.



## 2. Make a PR to publish the post
Start up your browser, connect to [akk1to/orz-blog](https://github.com/akk1to/orz-blog) and make a fork of the repository. Please remember that **we don't allow any PR to push into the `main` branch, except push to /src/blog (folder that contain posts)**. Only owner of the repository (akk1to.dev) and maintainers have the rights to maintain the `main` branch.
Navigate to the [`/src/content/blog`](https://github.com/akk1to/orz-blog/tree/main/src/content/blog) folder and then from there click the `Add file` button and selecting the `Upload files` button.
If it says you need to fork the repository, click the fork repository button and continue with the next steps on your forked repository.
Navigate to /src/content/blog then click Add file -> Upload files (Make sure to navigate to **/src/content/blog** before upload. Other folder will not work.)

<p align="center">
    <img src="https://i.imgur.com/iGIpIBr.png"></img>
    <p align="center"><i>Make a new fork of the repository</i></p>
</p>
<p align="center">
    <img src="https://i.imgur.com/rG3PsVd.png"></img>
    <p align="center"><i>Click "Add file" then "Upload files"</i></p>
</p>
<p align="center">
    <img src="https://i.imgur.com/cSYF3ux.png"></img>
    <p align="center"><i>Forked repository of orz-blog</i></p>
</p>

Next, drop your post file (.md format) into the upload box. You can name the file anything you want but make sure that you follow these requrements below:
- All required fields (e.g., author, description) are filled in without omissions.
- The file is saved in the `.md` format. Posts in any format other than Markdown will not be accepted.
- The content is written entirely in Markdown to ensure proper display.
- The file is located in the correct directory (`/src/content/blog`). Files placed elsewhere will not work.
- Images used in the post are hosted online (e.g., Imgur, Pexels). Locally hosted images are not supported.
- The post URL corresponds to the file name. For example, a file named `post-01.md` will generate a URL like `{blogdomain}/post-01`.
- Sample code included in the post must be functional and thoroughly tested. Posts with non-working code snippets will not be approved.
- The post must not contain sensitive information, racist content, nudity or sexually suggestive material, hate speech, credible threats, direct attacks on individuals or groups, references to self-harm, or depictions of excessive violence.
- Ensure adherence to the **Community Standards** when creating and publishing content on our blog platform.

```md
---
title: "Test post"
description: "hello this is a test post"
published: "1735273160000"
author: "akk1to.dev"
---
This is a test post so nothing here.
```
<p align="center"><i>test.md file</i></p>
<p align="center">
    <img src="https://i.imgur.com/hYajfIp.png"></img>
    <p align="center"><i>An example when upload post to the repository</i></p>
</p>

Make sure to select "Commit directly to `main` branch" then click "Commit changes".
After you have uploaded the file, navigate back to [akk1to/orz-blog](https://github.com/akk1to/orz-blog) and make a PR request, compare across your fork and the main repository.
<p align="center">
    <img src="https://i.imgur.com/Ya2Thg8.png"></img>
    <p align="center"><i>Make a PR, compare across base repository and head fork</i></p>
</p>

Then, click "Create pull request" and fill in neccessary information, place an `x` between the `[ ]` (so it looks like `[x]`) for each requirements you meet. Please make sure you meet all the requirements before creating the pull request. Make sure to check "Allow edits by maintainers".
Once you have filled out the requirements you can then click the `Create pull request` button and you're done!
<p align="center">
    <img src="https://i.imgur.com/lQjZBVg.png"></img>
    <p align="center"><i>Create pull request</i></p>
</p>
<p align="center">
    <img src="https://i.imgur.com/fknlP5z.png"></img>
    <p align="center"><i>An example Pull Request</i></p>
</p>

## 3. Waiting...

Since you have created your pull request, you will need to wait for a maintainer ([kodomotachi](https://kodomotachi.github.io/) or [akk1to.dev](https://akk1to.is-a.dev)) to merge it before you post becomes active. Make sure to keep an eye on your pull request incase one of the maintainers requests changes.
**_Your pull request will normally be merged with-in 12-24 hours, however in some cases it may take longer. Please be patient as the maintainers are very busy._**
Once your pull request is merged you should be good to go! Now your post will active at https://orz-blog.vercel.app/(filename) (delete .md tag).
Congratulations you have successfully post a new blog on our page!

<p align="center">
    <img src="https://i.imgur.com/TU3rhJ5.png"></img>
    <p align="center"><i>Accepted PR</i></p>
</p>

You can see this example post on https://orz-blog.vercel.app/test

_Make sure to join our [Discord server](https://wdh.gg/WxDO6wi) for announcements regarding the service._
