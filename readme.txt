=== WP Photo Sphere Smooth ===
Contributors: Jeremy Heleine, Allen Lew
Tags: Google, Android, Photo Sphere, photos, panoramas, 360-degree, equirectangular
Requires at least: 3.1
Tested up to: 4.2.1
Stable tag: 3.1
License: MIT
License URI: http://opensource.org/licenses/MIT

A filter that displays 360x180 degree panoramas.

== Description ==

<<<<<<< HEAD
WP Photo Sphere Smooth is a filter that allows you to display 360x180 degree panoramas. With WP Photo Sphere, your visitors will be able
=======
WP Photo Sphere Smooth is a filter that allows you to display 360x180 degree panoramas. With WP Photo Sphere Smooth, your visitors will be able
>>>>>>> origin/master
to navigate through your panoramas without install any plugin.

WP Photo Sphere Smooth is based on the JavaScript library [Photo Sphere Viewer](https://mistic100.github.io/Photo-Sphere-Viewer/) by [Damien Sorel](http://www.strangeplanet.fr/), a fork of [Photo Sphere Viewer](http://jeremyheleine.me/#photo-sphere-viewer) by [Jérémy Heleine](http://jeremyheleine.me/).

This plugin allows you to display equirectangular panoramas, taken with a classic camera or with Photo Sphere on Android and iOS.

If you want to contact me for any reason, feel free to email me at allen@alew.org or contact me on:

* Twitter: https://twitter.com/enlewof
* Google+: https://plus.google.com/+AllenLew09
* Facebook: https://www.facebook.com/allenlew

WP Photo Sphere Smooth is available in:

* English,
* French,
* Spanish,
* Portuguese (thanks to [Pedro Mendonça](https://github.com/pedro-mendonca)),
* Turkish (thanks to [Alper Demir](https://www.cesakozmetik.com.tr/)).

== Installation ==

1. Upload the `wp-photo-sphere` folder to the `/wp-content/plugins/` directory
2. Activate the plugin through the 'Plugins' menu in WordPress

== Frequently Asked Questions ==

= How to add a panorama? =

Use the `Add a panorama` button to upload or choose a panorama to insert into your post.

= Is it possible to read a distant panorama? =

Since version 1.0, it is possible to read a distant panorama located on another website thanks to its URL. To do that, do not
indicate any ID number and use the `url` attribute. Note that this feature does not work with domains that did not enable CORS.
For example: `[sphere url="http://upload.wikimedia.org/wikipedia/commons/a/a4/Cascading_Milky_Way.jpg"]`.

= How to change the title? =

The default title displayed on each WP Photo Sphere link can be changed in the options page. You can also choose to display an
unique title for a specific panorama by using the `title` attribute. Note that the `%title%` tag is also available in this
attribute.

= How to change the dimensions? =

By default, the dimensions are 560 x 315 pixels but you can change that in the options page (in the Settings menu).

You can also choose different dimensions for each panorama using the width and height attributes.
For example: `[sphere 42 width="200" height="400"]` or `[sphere 42 width="50%" height="300"]`.

A maximum width can also be given with the attribute max_width. Its default value can be changed in the options page.

= How to display the navigation bar? =

The navigation bar allows users to zoom, animate the panorama or view it in fullscreen. To display it, just use the `navbar` attribute
with the value `yes`: `[sphere 42 navbar="yes"]`.

You can choose to display it (or not) on all of your panoramas in the options page. If you display it on all of your panoramas and
want to deactivate it on one particular panorama, use the `navbar` attribute with the value `no`.

= Can I change the automatic animation? =

By default, panoramas are automatically animated after 2000 milliseconds, but you can change this with the
anim_after attribute. You can also deactivate the animation with the value -1. For example:
`[sphere 42 anim_after="5000"]` or `[sphere 42 anim_after="-1"]`.

You can set the animation speed with the anim_speed attribute. It accepts six units: revolutions per minute/second
(rpm/rps), degrees per minute/second (dpm/dps) or radians per minute/second (rad per minute/second). The default
speed can be set in the options page.
Example: `[sphere 42 anim_speed="10rpm"]`.

= Is it possible to autoload the panorama? =

Since the version 1.1, you can specify, for each panorama, a special attribute: `autoload`. If you use this attribute,
the panorama will start automatically after the page has loaded. This attribute doesn't require any value, for
example: `[sphere 42 autoload]` or `[sphere 42 width="300" height="150" autoload]`.

= How to change the levels of zoom? =

Minimal and maximal levels of zoom can be personalized in the options page by changing the minimal and maximal fields of view. You can
also use the `min_fov` and `max_fov` attributes.

== Screenshots ==

1. Options page
2. WP Photo Sphere link
3. Panorama

== Changelog ==

= 1.0 =
* First version forked from version 3.1 of original
