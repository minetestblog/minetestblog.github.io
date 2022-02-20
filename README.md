This is a periodic blog for sharing status updates with the minetest community. Check out the [about page] (https://minetestblog.github.io/about/)

## Workflow 

Blog editors have access to the repository. Their job is to curate the content submitted by the community and to create the periodic posts from the submitted content.

In the main directory, there are two important files:

`YYYY-MM-DD-sample_post.markdown`

and 

`YYYY-MM-DD-next_post.markdown`

The first is a basic template for each post, and the second is the staging area for the upcoming post. 

Do not change the names of the files; the website builder automatically ignores *those* particular file names.

The workflow is as follows: 

1) Delete last month's `YYYY-MM-DD-next_post.markdown`
2) copy `YYYY-MM-DD-sample_post.markdown` and rename it `YYYY-MM-DD-next_post.markdown`
3) Over the next month (or current period between posts), edit `YYYY-MM-DD-next_post.markdown` to contain the content for the next post:
  * as issues are submitted on the [github issue tracker] (https://github.com/minetestblog/minetestblog.github.io/issues) and on the mirrored [gitlab issue tracker] (https://gitlab.com/mistere123.coding/minetestblog.github.io/-/issues), Review the content provided in the issue and determine if it meets the [standards] (https://minetestblog.github.io/about/)

  * if it does, add it to the staging post. Organize the staging post by post type (headings are already given in the template). Include screenshots if they fit, and put a caption under them. We should only select 1 or 2 "Best of minetest" screenshots, and put them at the end of the post.
  * place images in the /_posts/img folder

  * close the issue as the content is added.

4) At the release time, Write a brief overview of the post in the overview section. Include the highlights only, not every detail. Choose or take a post cover image and link it in the header of the post. Also change the variables in the header as appropriate. Delete any headings in the post that do not have content, and their table of contents entry.

5) move the staging post into the _posts folder, and rename it to fit (`YYYY-MM-DD-postname.markdown`)

Thats it!


If you want to help out, and be an editor, we need you! Email MisterE at `mistere123.coding@gmail.com` 





# dactl - Our web theme
dactl is a fast, modern and configurable [Jekyll](http://jekyllrb.com/) theme with some tricks up it's sleeve. It has a live theme switcher and it's main blog layout display prominent hero images for posts with colored overlays and nice animations.

![light theme](uploads/screenshot_desktop_light.jpg)
![dark theme](uploads/screenshot_desktop_dark.jpg)

## License
All parts of dactl Jekyll theme are free to use and abuse under the open-source [MIT license](http://opensource.org/licenses/mit-license.php).

## TO DO
- [ ] Inline critical `.css` in `<head>` for faster load times
- [ ] Fix theme-switcher - sometimes it does not inject all of the colors properly on first page load and a refresh, fixes itself after switching the theme back and forth.

