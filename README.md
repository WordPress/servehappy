# WordPress php education initiative (codename `servehappy`).
[![Edit in GitHub](https://img.shields.io/badge/Edit_in_GitHub--green.svg?style=social)](https://github.com/WordPress/servehappy/edit/master/README.md)

The servehappy project is an initiative that seeks to educate WordPress site owners about the value of having the latest version of PHP powering their WordPress site.  This supports the overall goal of increasing percentage of WordPress installs running modern PHP versions.

## Background

One of the core tenets of WordPress has been that of being backward compatible and the support of PHP 5.2 is and has been part and parcel of that tenet.  Over the years however, there has been increasing tension within the WordPress developer community on this support for PHP5.2 between those who support keeping the minimum PHP version requirements the same for WordPress core, and those who want to increase the minimum PHP version requirements for WordPress core.  There have been numerous arguments made for either side and you can follow some of the discussion [here](https://core.trac.wordpress.org/ticket/33381).

Beginning around mid 2017, there were a number of discussions initiated (in various channels) about resolving some of this tension and keeping WordPress as a project moving forward with PHP language related topics. Out of these discussions, a number of initiatives were started that support the overall _initial_  goals of:

- encouraging Web host providers to provide the latest PHP versions and provide an upgrade path for their customers to get on the latest versions (this is something that has been happening for a while now)
- educating site owners about PHP and why PHP version matters.
- decreasing the amount of reported WordPress sites running older EOL versions of PHP.

Once these goals have been reached, then it becomes possible to more practically begin discussions about:

- increasing the minimum PHP requirements of WordPress
- introducing more modern PHP practices/design patterns etc that require later PHP versions in WordPress php code design and structure.

For clarity, its worth re-iterating here, that the immediate goal of the latest PHP initiatives (of which the _servehappy_ project is a part) is **not** to raise the minimum _requirements_ for PHP in WordPress core. The immediate goal is to put in place supporting structure and site owner education/resources etc so that we can more actively reduce the number of existing active WordPress sites on older PHP EOL versions.


## Following along

We will endeavour to keep this document up to date, but for all the most recent information you will want to follow along at:

* [Slack Channel](https://wordpress.slack.com/messages/core-php/)
* [Trac ticket](https://meta.trac.wordpress.org/ticket/2996)
* [Weekly updates](https://make.wordpress.org/core/tag/core-php/)

## Big picture overview

The following table gives a high level overview of all the various components contributing to the servehappy initiative.

> Note: all delivery dates are _rough_ estimates only.

| Deliverable | Links | Status | Est Delivery Date |
| ------------ | ---------- | ---------| -------------|
Benefit/Stats Collection | - [issue tracker](https://github.com/WordPress/servehappy/issues)<br> - [ Benefits & Stats project board](https://github.com/WordPress/servehappy/projects/1) | ongoing | TBD |
| Resource Collection | [the servehappy resources repository](https://github.com/WordPress/servehappy-resources) | ongoing | TBD |
| Information Page on WP.org | - [Current Draft](https://github.com/WordPress/servehappy/blob/master/DRAFT.md) <br> - [trac ticket](https://meta.trac.wordpress.org/ticket/2996) | **active** | 1st Quarter 2017 |
| Admin Notice in Dashboard | - [Create browse happy type notice for PHP versions](https://core.trac.wordpress.org/ticket/41191) | **active** | TBD |
| Minimum PHP version API for plugins/themes in core | - [trac ticket](https://core.trac.wordpress.org/ticket/40934) | **active** | TBD |

A more descriptive outline of some of the concrete deliverables associated with the servehappy initiative:

### Collection of Benefits and Stats

Ongoing collection of benefits and statistical data is used to help sell the "update PHP" proposition to users.  These have been collected as issues in the [issue tracker](https://github.com/WordPress/servehappy/issues) and managed in the [ Benefits & Stats project board](https://github.com/WordPress/servehappy/projects/1).

If you want to suggest a new benefit or stat, please [create a new issue](https://github.com/WordPress/servehappy/issues/new) and label it accordingly.

### Collection of various third-party articles and hosting resources

See [the servehappy resources repository](https://github.com/WordPress/servehappy-resources) where there is an ongoing effort to collect a resource library of third-party articles, and php upgrade tutorials (including host specific tutorials) that can be utilized in other resources developed as a part of this initiative.

### Information page about PHP versions and updates.

This page will live on WordPress.org and is intended to be referenced throughout the WordPress.org project and eventually linked to from the WordPress dashboard for sites not meeting a minimum PHP version requirement.

* [Current Draft](https://github.com/WordPress/servehappy/blob/master/DRAFT.md)
* https://meta.trac.wordpress.org/ticket/2996

### Admin notice in WordPress Dashboard

This admin notice will serve as a portal into more substantive educational pieces (linking through to the [Information page about PHP versions and updates](#information-page-about-php-versions-and-updates)).

* [Create browse happy type notice for PHP versions](https://core.trac.wordpress.org/ticket/41191)

### Minimum PHP version API for plugins/themes in core

The proposal is to allow plugins and themes to have a minimum PHP version requirement. This will involve work done in WordPress core and the WordPress.org plugin repository to support this. More details can be tracked via the [trac ticket](https://core.trac.wordpress.org/ticket/40934)

## Tide Project

While not directly related to the servehappy initiative, the [Tide Project](https://make.wordpress.org/tide/) will indirectly support the various efforts in process.  It will particularly help with prividing feedback to users about what plugins/themes they have in use on their site that might not be compatible with a PHP version being upgraded to.

- see [here](https://xwp.co/tide-a-path-to-better-code-across-the-wordpress-ecosystem/) for an overview of what the tide project is

## Related Trac tickets/Other Resources

This is a list of trac tickets that have some relation to the overall servehappy project:

- https://core.trac.wordpress.org/ticket/33381
