# Integrating the Servehappy Page with WordPress Core

[![Edit in GitHub](https://img.shields.io/badge/Edit_in_GitHub--green.svg?style=social)](https://github.com/WordPress/servehappy/edit/core-integrations/CORE-INTEGRATIONS.md)

## Integration Points

### Admin Notice

If the site is using a PHP version which is no longer supported, a dismissible notice should display to site administrators, indicating that they should upgrade the version. That notice should include a brief summary of the issue and then link to the Servehappy page for more education and, more importantly, instructions on how to prepare and perform the PHP upgrade.

*Core Trac Ticket: [#41191](https://core.trac.wordpress.org/ticket/41191)*

### Admin Footer

In addition to showing the WordPress version the site is running, the PHP version should be displayed. If it is no longer supported, a link to the Servehappy page should be shown instead, similar to the current link for updating WordPress, with an anchor text such as "Upgrade to PHP 7.2".

*Core Trac Ticket: TODO*

### Plugin Requirements

If the site administrator wants to install or update a plugin that requires a higher PHP version than the site is running on, the process should be prevented. The plugin should be highlighted in a way that this is easily recognizable and the respective buttons should be disabled. There should be a small link-like button such as "Why?" that, when clicked, toggles a small notice stating that the PHP version is too old to run the plugin, including a link to the Servehappy page for further help.

*Core Trac Ticket: [#40934](https://core.trac.wordpress.org/ticket/40934)*

## Links

Links to the Servehappy page from WordPress core should preferably include certain GET parameters, such as the PHP version active and the context of why the page is being linked to, referring to one out of the integration points above. The Servehappy page could then serve more targeted content, particularly in the introduction section, making it easier for the user to relate their problem.

## Scope

Generally, notices and links should only display if the PHP version used is no longer supported. However, in order to reduce the maintenance burden and efforts for hosts, there should be multiple iterations, with the first step showing the notice only on those sites running on PHP 5.2.

In contrast to that, PHP version requirements of plugins are independent of specific PHP versions and should always display as needed. Even a site already on PHP 7.0 could see such a notice if a plugin required PHP 7.1 or 7.2 - this is however unlikely and mostly theoretical.

## Recommended Version

The Servehappy page should always recommend a specific PHP version, such as "PHP 7.2 or greater", and stay away from less precise variants like "a supported PHP version". That version should always match what is recommended on the [WordPress Requirements page](https://wordpress.org/about/requirements/).

Core itself however should not use specific PHP versions as it should be possible to change the recommended version without updating WordPress. This may be reevaluated if there was an API exposing the recommended PHP version so that each WordPress install could gather that information remotely.

## Maintenance Burden

While updating the recommended version is only a small maintenance burden at this point, with the introduction of the Servehappy page and integration with core more areas will now reference that version specifically. A good idea would be to have a central location in the wordpress.org infrastructure to set that version. It could be a simple setting, and there could be a shortcode to include that version anywhere on wordpress.org. In addition, the wordpress.org API could also include that version somewhere which would allow WordPress core to be more specific about upgrade recommendations as well.