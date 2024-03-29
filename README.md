# Newspack WooCommerce Memberships Auto-archive

This plugin is an extension of the WooCommerce Memberships.

It provides "premium archive content" to your WordPress/Newspack web site.

The posts are kept public until a number of days you get to define, after which they automatically become Restricted Content. This behavior can be turned on or off, and customized per post.

## Installation

Download the latest `.zip` file from Releases, and install on your WordPress / Newspack site. Make sure to first install WooCommerce Memberships, since this plugin doesn't work without it. 

## Development

To get set up for development, run `npm install && npm start`.

## Usage

This plugin adds a simple Pannel to the Block Editor document settings side bar.

When the feature is turned on, it first sets public access to the Post. After the defined number of days, it automatically turns the Post to restricted content. 

When the Post becomes Restricted Content (gets archived) it will get all the Restriction Rules defined in your Memberships Plans.

### Integration with Memberships Plans

The WooCommerce suite enables a wide variety models of product sales. 

In order to use "premium archive content" on your web site, the Memberships Plans need to be tuned to this Plugin's purpose. When setting up your Memberships Plans rules, consider you will want certain Plans to gain access both after the post has become archive, and during it's public.

A simple Membership Plan setup to work with this plugin could be:
- in WordPress Admin zone, go to `WooCommerce` > `Membersips` > `Membership Plans`
- for a specific Membership Plan, you could add a rule such as: Type "Posts", Accessible "Immediately"

Member using plan will be able to see the post while it's public, and also when it gets archived (promoted to restricted content). 

