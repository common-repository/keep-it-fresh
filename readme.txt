=== Keep it Fresh ===
Contributors: jonkern
Donate link: http://www.jonathankern.com/code/keepitfresh
Tags: posts, filter, old, archive
Requires at least: 2.7
Tested up to: 2.9
Stable tag: 1.0
Text Domain: keepitfresh

Keep it Fresh will stop WordPress from showing posts older than a set number of days or a specific date.

== Description ==

Keep it Fresh will stop WordPress from showing posts older than a set number of days or a specific date. It is configurable via the WordPress administration area. Keep it Fresh doesn't remove old posts, nor does it muck with their `post_status`; rather, Keep it Fresh uses the `posts_where` WordPress filter to filter out posts older than the given date or amount of days whenever WordPress requests posts outside of the admin area.

== Installation ==

1. Upload the `keep-it-fresh` folder to the `/wp-content/plugins/` directory
1. Activate the plugin through the 'Plugins' menu in WordPress
1. Setup Keep it Fresh as you please via the Keep it Fresh options page under Settings in the WordPress admin area

== Frequently Asked Questions ==

= How does Keep it Fresh hide my old events? =

Keep it Fresh adds a date filter on the posts query each time WordPress requests posts to display (except when in the admin area).

= `get_posts` still returns old posts. What do I do? =

The `get_posts` function will suppress the filters that Keep it Fresh uses to hide old posts by default. To avoid this behavior, pass an array to `get_posts` with the key `suppress_filters` set to false. For example: `get_posts(array('suppress_filters'=>false))`.

= I love Keep it Fresh, but I'd like it to do &lt;blank&gt;. =

Great, I'm glad to hear feature requests.  Just post a comment on the [plugin's homepage](http://www.jonathankern.com/code/keepitfresh "Keep it Fresh Homepage").

== Changelog ==

= 1.0 =

* Initial Release