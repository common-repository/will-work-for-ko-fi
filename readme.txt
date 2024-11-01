=== Will Work for Ko-fi ===
Contributors: mlchaves
Donate link: https://ko-fi.com/marklchaves
Tags: button, donation, kofi, cgb, block
Requires at least: 5.3.2
Tested up to: 5.8.1
Stable tag: 2.1.1
Requires PHP: 7.2
License: GPLv2 or later
License URI: https://www.gnu.org/licenses/gpl-2.0.html

Custom Gutenberg Block (CGB) for the Ko-fi donation button.

== Description ==

Welcome to the Will Work for Ko-fi (WW4KOFI) Gutenberg block version 2.0.0.

Add your customised official Ko-fi button to your posts and pages. Visually preview your customisations in the block editor.

This custom Gutenberg Block (CGB) for the Ko-fi donation button allows you to:

1. Create an optional heading
1. Add a short call-to-action prompt
1. Insert your custom button text
1. Choose a background colour using a built-in colour picker 
1. And of course, add your Ko-fi _code_ or username

== Installation ==

1. Upload the contents of the plugin zip file to the `/wp-content/plugins/will-work-for-ko-fi` directory, or install the plugin through the WordPress plugins page directly.
1. Activate the plugin through the 'Plugins' page.

== Usage ==

1. Open a page or post in Gutenberg.
1. Click on the `+` to add a block.
1. Start typing "Will Work for Ko-fi" until you see the block appear, then select it.
1. Inside the block, enter an optional heading or short description into the respective input fields.
1. In the settings sidebar, enter the text you want on your button. This is important! Keep it short.
1. In the settings sidebar, use the colour picker for the button's background.
1. Remember to enter your Ko-fi _code_ or username. This is also in the settings sidebar.
1. Preview, Update, or Publish your page or post and enjoy ;-)

== Frequently Asked Questions ==

= Is WW4KOFI v2 lightweight? = 

Yes. It's only 47 KB zipped. And, it uses its' own local copy of the official Ko-fi widget JavaScript library.

= Is the Ko-fi button the official button from ko-fi.com? =

It sure is. The Ko-fi button widget code comes from https://ko-fi.com/manage/widgets and it looks like this.

`
<script type='text/javascript' src='https://ko-fi.com/widgets/widget_2.js'></script><script type='text/javascript'>kofiwidget2.init('Support Me on Ko-fi', '#29abe0', 'D1D7YARD');kofiwidget2.getHTML();</script> 
`

= How can I change the alignment for the Will Work for Ko-fi block? =

You can change the content alignment by using [additional CSS](https://medium.com/@marklchaves/adding-custom-css-to-your-wordpress-website-how-to-guide-a50b474af36d). The additional CSS below will centre justify the WW4KOFI block contents.

`
.centre-this-block {
	text-align: center;
	width: 50%;
	margin: 0 auto;
}
`

= How can I change the style of the Will Work for Ko-fi block? =

You can change the content alignment by using [additional CSS](https://medium.com/@marklchaves/adding-custom-css-to-your-wordpress-website-how-to-guide-a50b474af36d). The additional CSS below will add slight padding to the contents and create a drop shadow effect.

`
.style-this-block {
	padding: 1.5%;
	border-radius: 10px;
	box-shadow: 5px 20px 12px rgba(0,0,0,.2);
}
`

Version 2.1.0 introduced the `.section__kofi` CSS class that controls the top/bottom padding for the widget's heading, description, and button.

`
.section__kofi {
  padding-top: 0;
  padding-bottom: 0;
}
`

= Do I need to install the Lazy Blocks plugin too? =

No. Version 2.0.0 does not rely on any third-party plugins. Lazy Blocks is deprecated in v2.0.0.

= I'm seeing a "This block contains invalid or unexpected content" error message. What must I do to fix it? =

Click on the horizontal ellipses (...) on the right, then select **Attempt Block Recovery**.

== Screenshots ==

1. Your very own **personalised** official Ko-fi button.
1. Get creative with your button placement and styling.
1. Style your Will Work for Ko-fi block with custom CSS.
1. NEW live button preview in the block editor. Customise the heading and description in the editor. Edit the button text, button colour, and Ko-fi ID in the block inspector.
1. Use additional CSS for custom styling. Add your CSS class names under the **Advanced** section in the settings sidebar.

== Changelog ==

= 2.1.1 =
* Added local Ko-fi image assets.
* Tested with WordPress 5.7.1.

= 2.1.0 = 
* CSS changes. Mainly to add section class to avoid inheriting large padding used in Twenty Twenty theme CSS.
* Tested with WordPress 5.6.

= 2.0.0 = 
* Added support for live preview of the Ko-fi button. The live preview displays inside the block while in the block editor.
* Moved the button text and button colour controls to the inspector (right sidebar).
* Removed the dependency for Lazy Blocks.

= 1.2.0 =
* Added proper use of enqueue for the official Ko-fi JavaScript library.
* Readme updates.

= 1.0.0 =
* First release. Tested on the Twenty Twenty and GeneratePress themes.

== Upgrade Notice ==

= 2.0.0 = 
* Version 2.0.0 is nearly a complete rewrite. 
* Version 2.0.0 is now only 47 KB zipped. Version 1.* was almost 1 MB zipped because of the Lazy Blocks dependency.

= 1.2.0 =
* Upgrade to ensure that the Ko-fi widget JS library is properly enqueued to meet WordPress developer standards.
* Removed separate install requirement for Lazy Blocks. Lazy Blocks is included in the Will Work for Ko-fi plugin install.

= 1.0.0 =
None

== Credits ==

Built with [Create Guten Block](https://github.com/ahmadawais/create-guten-block).

_Will Work for Ko-fi_ coffee logo by walkerstudio13 from the [Noun Project](https://thenounproject.com/search/?q=coffee&i=2491285).