# Clarity Ghost Theme

`clarity` is a  [MathJax](http://www.mathjax.org) ready [Pure](http://purecss.io) based theme for [Ghost](http://github.com/tryghost/ghost/).
It is already integrated with [microdata](https://support.google.com/webmasters/answer/176035?hl=en) for search engine optimization and opengraph for better facebook integration.

You can see a running version of the dark theme is on my blog [Tales of a Fractal Spectrum](https://danjpark.com).

Please note that this new version integrates some changes of Ghost 1.6.* and will not work on older installations. **Consider upgrading Ghost to version 1.6.0 before upgrading the theme!**

## What does the ZIP contain
The zip contains the full theme with a detailed README.

It is ready to be integrated with your favorite social networks, ready to be used with google+, disqus or Facebook comments and ready to be integrated with Google Analytics. Until this will be made automatic with the introduction of plugins in Ghost, you will find detailed instructions on the README file.

_For some of the following operations you need to edit css or hbs files. Use your favourite pure text editor for the purpose. Please avoid Office, LibreOffice/OpenOffice or similar suites._

## Install the theme
Decompress the zip file inside the folder `content/themes/` of your Ghost blog.
Or, go into Design on your http://yourblog.com/ghost/ and load in the zip file.

## Update your social network informations
Open the file `default.hbs` and look for the following lines

```
	<ul class="social-list">
			<a href="https://www.github.com/.../" target="_blank"><i class="fa fa-github-alt" aria-hidden="true"></i></a>&nbsp;
			<a href="https://www.linkedin.com/in/.../" target="_blank"><i class="fa fa-linkedin" aria-hidden="true"></i></a>&nbsp;
			<a href="https://www.instagram.com/.../" target="_blank"><i class="fa fa-instagram" aria-hidden="true"></i></a>&nbsp;
            <a href="{{@blog.url}}/rss/" target="_blank"><i class="fa fa-rss" aria-hidden="true"></i></a>
	</ul>
```

The `fa fa-SocialNetworkName` identifies which icon is used and more details can be found by visiting http://fontawesome.io/
Duplicating those line and editing the name of the icon and the link will add additional social networks. For the full list of supported icons, please refer to the font awesome website.

## MathJax support
To enable MathJax (if you don't know it, probably you don't need it) it is enough to open the file `default.hbs` and completely delete the two lines containing the text `REMOVE THIS LINE TO ENABLE MATHJAX`.

## Google Analytics support
After having obtained your Account Code from [analytics.google.com](http://analytics.google.com), it is a code of the form `UA-12345678-1`, open the file `default.hbs`, completely delete the two lines containing the text `REMOVE THIS LINE TO ENABLE GOOGLE ANALYTICS` and replace `REPLACE_THIS_TEXT_WITH_THE_ACCOUNT_NUMBER_GIVEN_BY_GOOGLE` with your account code.

## Google+, Disqus or Facebook comments
To set up google+, disqus or facebook comments is enough to open `posts.hbs`, and remove the appropriate lines at the end of the file (they are marked with `REMOVE THIS LINE TO ENABLE ...`). 
For [Disqus](http://disqus.com) you additionally need to register to their website and obtain a website identifier.
You can add the Comments counter on the index page modifying the code according to [Another way of enabling disqus on Ghost](http://blog.reggiesuplido.com/another-way-of-enabling-disqus-on-ghost/).

## Support
