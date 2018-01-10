# Why should you upgrade your PHP version for WordPress

[![Edit in GitHub](https://img.shields.io/badge/Edit_in_GitHub--green.svg?style=social)](https://github.com/WordPress/servehappy/edit/master/DRAFT.md)

Does your website seem to run slow? Are you losing customers because of page speed? Is Google lowering your ranking? It’s possible your server software is outdated.

Your website might not be operating at its full potential. This page will tell you about an important issue your site might be suffering from and how to resolve it. Let's talk about what PHP is, and why you might need to update it.

[The above section should display alternative, more targeted content if a GET parameter is present indicating which version the user visiting the page is running on their site. WordPress core links could easily include such a parameter.]

## What is PHP?

PHP is the foundational coding technology of WordPress. Just like any underlying structure, it’s important that it is strong and secure. When you use an old version of PHP on your WordPress host, you are building a WordPress site on weak bedrock. Upgrading to the latest version of PHP is crucial to ensuring your site is secure, fast, and compatible with all parts of WordPress. There are a number of great reasons why you should update to the latest version of PHP.

Currently, WordPress is tuned to use the latest version of PHP (linked to requirements page). Although WordPress’ commitment to backward compatibility allows you to use versions as old as PHP 5.2, that version of PHP was originally released in 2007. It’s so old, even the PHP people don’t maintain it anymore. Do you want your website to depend on ancient software?

## Why Should PHP Matter to You as a Site Owner

There are three things you should care about as a site owner. First, caring the site works as expected when people visit. This is generally referred to as “site availability.” You should also care about how fast the site loads and functions.  This is commonly called “performance.” Lastly, you should care that your site can make use of all the latest and greatest tools. We refer to these as “features.”

### Site Availability

Each of us has clicked on an ad or link that end up with 404 errors or the dreaded “white screen of death.” You spend a lot of time and effort to get people to click on your links, and when they have a bad landing page experience, all those marketing efforts go to waste. 
There are many reasons that this could happen, such as the server getting unplugged, internet connection issues or human error in configuration.  One of the scarier reasons a site could go down is because of hacking. WordPress is a safe and secure platform for your business, as long as you are keeping everything up to date. Unfortunately, bad people on the internet will figure out exploits of any code, and hack sites using that code. Since PHP is running a very large percentage of the web, and WordPress is built on PHP, these malicious people tend to focus their efforts on this underlying code. Once a vulnerability is publicly known, more bad actors use that same hole to attack more sites. 

Fortunately for all of us, the vibrant PHP community is constantly improving PHP. But the community members can only properly support the latest versions of the language. Older versions are not supported at all. Further streamlined: The code is freely available, so make sure to use the latest version to keep your site safe.

Keeping your PHP version up to date ensures your web site is ready for business, before your customers land on it.

### Performance

Your site needs to load fast enough to offer an enjoyable experience to your visitors. “73% of mobile internet users say that they’ve encountered a website that was too slow to load,” says Kissmetric’s research. They also say “40% of people abandon a website that takes more than 3 seconds to load.” Performance is also a key factor in determining your site's position in Google search results.

Just like any other complex machine, the performance of a site depends on the parts being of good quality and well tuned. PHP is a major part of how sites are delivered. One of the ways WordPress sites can improve performance without a lot of effort is to update PHP to the latest supported version, which is currently PHP 7.2. Sites can see a 30+% increase in performance by making this change.

### Features

Let’s imagine you are buying a state of the art car in 1978 vs today. Today, you would expect that a car would include audio as part of the stereo system, have heated seats, utilize active braking assistance, and include a rearview camera -- all standard. The car from 1978 would have none of those things. This doesn’t mean that it was a bad car; rather, the world of automobiles continued to progress and those features did not exist back then.  

WordPress has evolved much faster than automobiles and there are more new features available today than ever before. The newest features are only available in the newest version of PHP, so fewer features will be available to you if you don't keep up with the latest updates. Your options for features are going to be limited if you are not keeping up with the latest underlying updates. Make sure you can use the latest and greatest functionality for your WordPress website, and update to PHP 7.2.

## Are there risks when upgrading my PHP version?

In a perfect world, the answer would be “No”. However, the WordPress ecosystem is made up of thousands of themes and plugins (built and maintained by developers all over the world). All the various combinations of these parts that can be added to your site increase the potential for incompatibilities with certain PHP versions. WordPress cannot detect all those possible conflicts automatically.

WordPress as a content management system (CMS) is committed to backward compatibility. This means the main files that run your site will work as far back as PHP version 5.2. That said, we now recommend 7.2. Faster is better and this is why we’d love you to upgrade.

> **Aside:**
> “At Yoast we care about a lot of things, but two things in a very particular order: user happiness first, developer happiness second. A user is happy when he or she has a fast, easy to install, secure content management system like WordPress to build a site in. A developer is happy when he or she can use a modern language and modern tooling to build software with.” - [Joost de Valk - Whipping your hosting into shape](https://yoast.com/whipping-your-hosting-into-shape/)

## Before Upgrading PHP

### Backup & Rollback Plan

Before upgrading or making any major change you should create a backup of your site. This way you can easily restore your site should something go wrong. It happens. If you do not already have a backup solution in place, we recommend using [one of the free plugins](https://wordpress.org/plugins/search/backup/).
  
Though we are encouraging you to upgrade your version of PHP, it’s good to remind you that a standard WordPress backup only includes the database, media files, and code. The PHP version is set on the server level (by your website host) and is not included in the backup. Meaning, it would not automatically restore if you do need to restore. If upgrading to a higher PHP version causes issues, you will need to ask your host to move you back to the previous version of PHP. Read more in the  “Troubleshooting” section below.

### Standard WordPress Updates

Make sure all parts of your WordPress installation are updated. Update WordPress core and all of the plugins and themes that you are using. It is considered a best practice to update plugins and themes one at a time. This allows you to prepare yourself for any unexpected issue that could arise by pinpointing the problem plugin or theme.

> **Aside:**
> After you have successfully completed all of the available updates, it is useful to create and store a new backup in addition to the one from the first step, if your tooling allows for this. Most tools will let you create multiple backups that are either stored in the site’s file system or which you can download to your prefered storage solution such as your local computer or DropBox. This gives you a convenient rollback option to an intermediate step, so that you don't have to go through all updates again in case of a failure.

### PHP Compatibility Checker

One of the tools to guide whether or not a plugin is compatible with PHP 7.2 is the PHP Compatibility Checker. Install and activate the [“PHP Compatibility Checker” plugin](https://wordpress.org/plugins/php-compatibility-checker/) on your site. This can scan all plugins and themes for possible issues with modern PHP versions. After scanning your site, the plugin will give you the PHP version recommended to upgrade to and highlight any potential issues. As with all plugins, make sure to review the documentation (instructions). Also, as with any automated test, be aware that false positives are possible.

### Replace Incompatible Plugins

If you find one or more of your site’s plugins and themes do have real compatibility issues with the newer PHP versions, your options depend on how severe the issues are. Many incompatibilities can be fixed by a developer, sometimes requiring quick and simple changes. If you already have a developer of choice, ask them about this option. Otherwise, if a plugin or theme contains significant issues you need to find a replacement for it. Multiple plugins and themes with similar functionality that are compatible with the latest versions of WordPress can be found in the [WordPress plugin repository](https://wordpress.org/plugins/).

### Need Help?

Though these steps are straightforward and require just a little patience and persistence to implement, we realize that sometimes some people would like a little more help than just what the documentation provides. If you wish to find help with your PHP upgrade, these are your best sources:

* A Professional Web developer. If you have an existing relationship with a developer/agency, you may want to also consult with them regarding the specific needs for your site.
* Your Hosting Company. If you are on a host specializing in managed WordPress, they likely offer help with this process; we encourage you to ask.
* Plugin and theme authors. Don't hesitate to contact plugin and theme developers to request information about compatibility with a newer PHP version. Most of the time you can find their preferred support channel by looking at the plugin or theme itself in the admin screens. Most free plugins and themes are supported through the [official WordPress community support forums](https://wordpress.org/support/). For premium plugins or themes, you consult their terms of service and documentation.

## How to Upgrade PHP for your Website

While it would be stellar if WordPress could solve the PHP problem itself, that isn’t possible. PHP is part of the language on your website’s server and, unfortunately, WordPress is not in charge of the PHP version. It is up to you and your hosting provider.  

So how do you do it? Our favorite answer: it depends on how you are running your site. 

The good news is that many hosting providers will allow you to choose which version of PHP you can run. There are a lot of different companies with a lot of different ways to manage this.  Fortunately, the WordPress community has collected [some of the more popular providers’ upgrade paths](https://github.com/WordPress/servehappy-resources).  
If you cannot find instructions for your specific host, the best thing you can do is ask them. Here is a template  you can use when emailing your provider:

> Dear Hosting Provider,
>
> I want my website to be as performant and secure as possible with the latest version of PHP. For the server my WordPress site is hosted on, I want to ensure that is the case. If I am not already on the latest version of PHP, please let me know what steps I need to take to upgrade.

## Troubleshooting

**// TODO.**

## Conclusion

If your server isn't on the latest version of PHP, your website isn't operating at its full potential. 
Keeping foundational server-side software up-to-date is a great way to not only help your own website’s performance but to help keep the internet, as a whole, secure. Upgrade to PHP 7.2 today.
