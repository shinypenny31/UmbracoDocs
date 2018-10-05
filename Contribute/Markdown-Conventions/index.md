# Markdown conventions
The Umbraco Documentation uses Markdown for all of the documentation - but more precisely we use the CommonMark specification, read more about the difference [here](https://commonmark.org/).

## Structure
For the documentation project, each individual topic is contained in its own folder.
Each folder must have an `index.md` file which links to the individual sub-pages, if images are used, these must be in `images` folders next to the .md file referencing them relatively.

* topic
	* images
		* images.jpg
	* Subtopic
		* images
		* index.md
	* index.md
	* otherpage.md

## Images
Images are stored and linked relatively to .md pages, and should by convention always be in an `images` folder. So to add an image to `/documentation/reference/partials/renderviewpage.md` you link it like so:

	![My Image Alt Text](images/img.jpg)

And store the image as `/documentation/reference/partials/images/img.jpg`

Images can have a maximum width of **800px**. Please always try to use the most efficient compression, `gif`, `png` or `jpg`. No `bmp`, `tiff` or `swf` (Flash).

## External links
Include either the complete URL, or link using Markdown:

	https://yahoo.com/something

	or

	[yahoo something](https://yahoo.com/something)


## Internal links
If you need to link between pages, always link relatively, and include the .md extension.

	[Umbraco.Helpers](Umbraco.Helpers.md)

	or

	[Umbraco.Helpers](../../Reference/Umbraco.Helpers.md)

## Formatting code
Indent your sample with 4 spaces, which will cause it to be rendered as `<pre><code>` tags.
For inline code, wrap in ` (backtick) chars.

Use # for the headline, ## for sub headers and ### for parameters (on code reference pages)

For optional parameters wrap in _ (underscore) - end result: `###_optionalParameter_`