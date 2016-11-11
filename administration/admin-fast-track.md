Building your first Textpattern architecture \[todo:dw\]
========================================================

This will integrate the FAQ: ive-installed-textpattern-now-what.textile

This is a fast-track orientation to help you build your first publishing
architecture in Textpattern. It assumes you've [installed, configured,
and diagnosed a new instance of Textpattern](installation/intalling-txp)
on your web server and looked over the [administration](administration/)
docs. If you've done that but nothing more, you're now in a good place.
This orientation will map out the administration process and associated
locations in the administration side for building a single-author blog
system. The same mechanics would be followed for any other kind of
website, with adjustments to content types and functionality needed. But
exploring more content types and functionality gets into more advanced
Textpattern topics (not to mention requires planning your content model
and information architecture), which you are not ready for yet. So we'll
kick-start you with a basic blog model and you learn the rest like
everyone else does -- by reading more users docs, asking questions in
the [support forum](http://forum.textpattern.com), and exploring on your
own (the best kind of learning).

On this page:

-   "":\#sec1
-   "":\#sec2
-   "":\#sec3
-   "":\#sec4
-   "":\#sec5
-   "":\#sec6

Blog structure {#sec1}
--------------

Textpattern building blocks {#sec2}
---------------------------

below this line still needs editing

**Recommended reading:**

-   [sed\_cleaner](https://github.com/netcarver/sed_cleaner) (Plugin for
    one-time use immediately after setting language in a
    new installation. In one pass, it removes obsolete admin-side
    features and example content, and resets ID numbers for content
    types, among other nice things.)

### System security and troubleshooting {#system-security-and-troubleshooting .sectionedit2#system_security_and_troubleshooting}

The next step is to go the
[diagnostics](/home/www/zendstudio/dokuwiki/bin/doku.php?id=diagnostics)
panel where you'll see a few items in red that need clearing up
following a new install. New install errors are standard procedure to
let you know to delete the setup folder (if you haven't already), and to
create write permissions on the *tmp* and *files* folders in the [file
tree](/home/www/zendstudio/dokuwiki/bin/doku.php?id=ftp_installation_and_upgrading#file_tree).
The error diagnostics will be explanatory about what you need to do in
each case.

### User accounts {#user-accounts .sectionedit3#user_accounts}

Since user accounts are rather important for being able to do anything
at all, it makes sense to go have a look at the
[users](/home/www/zendstudio/dokuwiki/bin/doku.php?id=users) panel next.
Here is where you change your password and email address. And if other
users will have access to the admin-side, this is where you'll create
and edit their account details too, including
[user\_roles\_and\_permissions](/home/www/zendstudio/dokuwiki/bin/doku.php?id=user_roles_and_permissions).

**Recommended reading:**

-   [smd\_faux\_role](http://textpattern.org/plugins/1159/smd_faux_role)
    (Plugin for testing which user roles grant or restrict permission to
    which parts of the Textpattern administration, without needing to
    create roles and logging out and back in.)
-   [rah\_change\_passwords](http://rahforum.biz/plugins/rah_change_passwords)
    (Plugin allowing direct password management. Avoids the system
    generating random passwords and sending them by email.)
-   [smd\_bio](http://textpattern.org/plugins/1116/smd_bio) (Plugin that
    extends user account data collected and stored for custom output.
    *E.g.*, team profiles.)
-   [smd\_user\_manager](http://textpattern.org/plugins/1229/smd_user_manager)
    (Plugin providing user, group, and privilege
    management capabilities. Integrates with smd\_bio.)

### Site identity and default configurations {#site-identity-and-default-configurations .sectionedit4#site_identity_and_default_configurations}

With your installation secure, and your password in place, you should
set a few defaults that will influence the website's identity and
base-line publishing behaviour. You do this in
[basic\_preferences](/home/www/zendstudio/dokuwiki/bin/doku.php?id=basic_preferences),
which is the default screen of the *Preferences* panel. The other two
screens being
[advanced\_preferences](/home/www/zendstudio/dokuwiki/bin/doku.php?id=advanced_preferences)
and
[language\_preferences](/home/www/zendstudio/dokuwiki/bin/doku.php?id=language_preferences),
the latter you've already been to.

**Recommended reading:**

-   [basic\_preferences](/home/www/zendstudio/dokuwiki/bin/doku.php?id=basic_preferences)
-   [advanced\_preferences](/home/www/zendstudio/dokuwiki/bin/doku.php?id=advanced_preferences)

### Establishing site structure and design {#establishing-site-structure-and-design .sectionedit5#establishing_site_structure_and_design}

You're now ready to start assembling your basic site structure. As
mentioned at the start, we'll demonstrate the workflow by setting up the
home page, a blog section, and a basic archive for blog articles.

[pages](/home/www/zendstudio/dokuwiki/bin/doku.php?id=pages),
[styles](/home/www/zendstudio/dokuwiki/bin/doku.php?id=styles),
[sections](/home/www/zendstudio/dokuwiki/bin/doku.php?id=sections)

### Building publishing behaviour {#building-publishing-behaviour .sectionedit6#building_publishing_behaviour}

\[Categories, Forms, Tag builders\] (adding in the publishing
architecture to the layout in \#3)

### Managing content {#managing-content .sectionedit7#managing_content}

\[Write, Articles, Images, Links, Files, comments\] (routine publishing
for the Blog in \#3; invent a simple scenario)

### Extending with plugins {#extending-with-plugins .sectionedit8#extending_with_plugins}

\[Plugins, Extensions, etc\] (highlight some popular plugins used in
relation to the topics already covered; e.g. discussion of
smd\_bio/smd\_user\_manager in relation of user accounts)

### Monitoring referrers {#monitoring-referrers .sectionedit9#monitoring_referrers}

[visitor\_logs](/home/www/zendstudio/dokuwiki/bin/doku.php?id=visitor_logs)

**Recommended reading:**

-   [rah\_unlog\_me](http://rahforum.biz/plugins/rah_unlog_me) (Plugin
    that removes the administrators IP, and any others defined, so their
    site visits don't show up in visitor logs. Result is a more
    representative reflection of actual referrers that count.)

### Similar reading {#similar-reading .sectionedit10#similar_reading}

-   [Textpattern
    quickstart](/home/www/zendstudio/dokuwiki/bin/doku.php?id=textpattern_quickstart:hello_world)
