# Custom Background Extended #

Create custom backgrounds on a per-post basis.

## Description ##

A plugin for allowing users to set a custom background on a per-post basis.  This plugin hooks into the WordPress `custom-background` theme feature and overwrites the values on single post views if the post has been given a custom background.

### Features ###

This plugin creates a custom meta box on the edit post screen.  From that point, you can select a custom color and/or image.  If you select an image, you'll be presented with additional options for how the image appears on the site.

## Installation ##

1. Upload the `custom-background-extended` folder to your `/wp-content/plugins/` directory.
2. Activate the "Custom Background Extended" plugin through the "Plugins" menu in WordPress.
3. Edit a post to add a custom background.

## Frequently Asked Questions ##

### Why was this plugin created? ###

I've always been interested in art direction on blogs.  This is just one tool of many that I'm creating and making available via my [Web site](http://themehybrid.com "Theme Hybrid") for making it easier for users to take more control over their styles on a per-post basis.

### Why doesn't it work with my theme? ###

Most likely, this is because your theme doesn't support the WordPress `custom-background` theme feature.  This plugin requires that your theme utilize this theme feature to work properly.  Unfortunately, there's just no reliable way for the plugin to overwrite the background if the theme doesn't support this feature.  You'll need to check with your theme author to see if they'll add support or switch to a different theme.

### My theme supports 'custom-background' but it doesn't work! ###

That's unlikely.  Just to make sure, check with your theme author and make sure that they support the WordPress `custom-background` theme feature.  It can't be something custom your theme author created.  It must be the WordPress feature.

Assuming your theme does support `custom-background` and this plugin still isn't working, your theme is most likely implementing the custom background feature incorrectly.  However, I'll be more than happy to take a look.

### How do I add support for this in a theme? ###

Your theme must support the [Custom Backgrounds](http://codex.wordpress.org/Custom_Backgrounds) feature for this plugin to work.

If you're a theme author, consider adding support for this if you can make it fit in with your design.  The following is the basic code, but check out the above link.

	add_theme_support( 'custom-background' );

### Does it support custom post types? ###

The plugin supports WordPress posts and pages out of the box.

Because it's impossible for me to accurately determine what a **custom** post type should do, I've left it up to those of you actually building custom post type plugins to support this.  If you'd like to allow custom backgrounds on singular views of your post type, add `'custom-background'` to your post type `supports` array during registration.  Obviously, your post type would need to be publicly queryable and display something on the front end for single post views. 

Or, if you have a plugin with post types that you'd like for me to add support for, let me know.  I'll be more than happy to add the support via this plugin.

### Can you help me? ###

Unfortunately, I cannot provide free support for this plugin to everyone.  I honestly wish I could.  My day job requires too much of my time for that, which is how I pay the bills and eat.  However, you can sign up for my [support forums](http://themehybrid.com/support) for full support of this plugin, all my other plugins, and all my themes for one price.

## Changelog ##

### Version 0.1.0 ###

* Everything's new!