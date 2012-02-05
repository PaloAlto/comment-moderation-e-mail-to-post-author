=== Comment Moderation E-mail Only to Post Author ===
Contributors: RavanH
Donate link: https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=ravanhagen%40gmail%2ecom&item_name=Comment%20Moderation%20E-mail%20to%20Post%20Author&item_number=0%2e1&no_shipping=0&tax=0&bn=PP%2dDonationsBF&charset=UTF%2d8&lc=us
Tags: comments, moderation, comment, e-mail, author, comment notification, moderation queue
Requires at least: 3.1
Tested up to: 3.3.9
Stable tag: 0.2

Makes WordPress send the comment moderation notification *only* to the posts author's e-mail address and no longer to the main site admin e-mail address.

== Description ==

This plugin could also have been called "Don't bother Site Admin with Moderation Messages", unless admin is also the author...

When a comment gets posted to a particular post, the author of that post gets a notification about it. However, when that comment is held for moderation, the moderation notification is sent both to post author (if he/she has moderation rights) and the to the sites **Administrative moderator E-mail address** as configured under **Settings > General**.

For many blog or site owners, this might boil down to the same thing. But for **colaboration sites** where different people post, this might result in overflooding the admins mailbox with moderation messages that are not his/hers to moderate. The site owner, with enough on his/her mind already, is bothered with each and every new comment in the moderation queue.

This plugin changes that. **Just install, activate it and it's done...** All post comment moderation notifications will be sent **only** to the respective **Post Author**. If, by any chance, the post author has no moderation rights *or* there is no author e-mail set, the default site admin e-mail will be used.

Works on WordPress 3.1 and above in both Normal and Multi-site mode.

== Installation ==

Hit [install now](http://coveredwebservices.com/wp-plugin-install/?plugin=comment-moderation-e-mail-to-post-author), provide your site home address and continue to log in on your own site. Easy, by Covered Web Service :) 

== Frequently Asked Questions ==

= I see no settings page =
There is no settings page. The plugin will do only *one thing* : make comment moderation notifications go to the authors e-mail address, and no longer the site moderator address. 

= Nothing looks different. Is it working at all? =
To test if it is working:

1. Check your Settings > Discussion settings and make sure that (I) at **E-mail me whenever** at least *A comment is held for moderation* and (II) at **Before a comment appears** at least *Comment author must have a previously approved comment* are checked.
2. Log out and clear your browser cookies & cache.
3. As an anonymous visitor, post a comment to a post from anyone other than the main site owner.
4. Log back in, verify that comment went into the moderation queue and then ask the author if he/she received a moderation notification about it :)

= Does this plugin work on WPMU / WP3+ Multi Site mode? =
Yep. You can install it in /plugins/ and activate it *site-by-site* or *network wide*. Or you can opload it to /mu-plugins/ for automatic (Must-use) inclusion.

== Upgrade Notice ==

= 0.2 =
WP 3.1+ compatibility: no more messages to admin.

== Changelog ==

= 0.2 =
WP 3.1+ compatibility

= 0.1 =
First concept: replace function wp_notify_moderator()
