\\n[mininav\_content\_index](/home/www/zendstudio/dokuwiki/bin/lib/exe/fetch.php?id=&media=mininav_content_index)

[![](/home/www/zendstudio/dokuwiki/bin/lib/exe/fetch.php?media=file:tab_content-comment.png)](/home/www/zendstudio/dokuwiki/bin/lib/exe/detail.php?id=&media=file:tab_content-comment.png)

The **Comments** panel provides control about *visitor comments* on your
public pages. There are three modes of the panel

-   the primary (and default) *comments catalogue* for basic info and
    instant handling of comments
-   an edit mode where you can edit the comments content.
-   a list of banned IPs.

When opening the Comments panel you will get a \*catalogue\* of recent
comments, the latest comment at the top. Above the catalogue you'll find
a link “List banned IPs” which will show a list of IPs you banned in
your textpattern install. We'll describe this function later and begin
with the comments catalogue:

### Comments catalogue {#comments-catalogue .sectionedit1#comments_catalogue}

As in the other content panels catalogues can get pretty long after some
time. So as the first function there is a Search or Filter function:

#### Search and Filter {#search_and_filter}

The “Search” dialogue has two components:

-   A drop-down-list which lets you specify which area is to be searched
    or filtered
-   and a textfield for entering a search query or filter criteria.

Text entered in the textfield will be treated as a phrase, so search
results must exactly match the whole phrase. There is no OR or other
boolean search. You don't need to wildcard query text at the beginning
or the end (e.g. “time” will find “parttime”, “times”, “timestamp” as
well).

After entering your search phrase you start searching by clicking “Go”.
As a result you will be given a new catalogue of comments which meet the
criteria.

By default the search will find entered text in the articles' message.
But you can do more refined searches by selecting another area to search
in. The drop-down-list left from the textarea provides the following
search areas:

-   ID\#
-   Parent
-   Name
-   Message (default)
-   E-mail
-   Website
-   IP

Example: You can search a comment by any word in its message, if you
choose “Message” and type the word. Or you can filter the list and show
all comments from one person by choosing “Name” and typing an essential
part of the name (normally you needn't type the whole name).

#### The Catalogue {#the_catalogue}

Each row is a cooment. The columns list basic information about the
comment. The columns can be sorted. If you click the header of a column,
it will sort the comments according to that column. Click again to
reverse sort direction. The current sort column is marked by a yellow
arrow on the right side of its name indicating its direction.

The default view of the columns list:

**ID\#** - provides an ID for each comment.

**Date** - when the comment has been entered

**Name** - of the commentator

**Message** - The first words of the message (cropped)

**Parent** - The title of the article the comment has been written to.
If you click on the provided link, the article will open in the “Write”
panel.

By marking “Show Detail” there will be additional columns in the list:

**E-mail** **Website** **IP** **Status**

You will also find two additional links:

-   “Edit” will open an edit-window with the comment filled in.
-   “View” will show the comment on the public-side.

#### Hide Spam {#hide_spam}

By default Textpattern will hide comments which are automatically
identified and marked as “spam”. By marking “Show Spam” spam comments
will be visible in the catalogue.

### List of banned IPs {#list-of-banned-ips .sectionedit2#list_of_banned_ips}

If you follow the links “List banned IPs” the panel will change into the
IP-list-mode. You will see a list of banned IPs. each row is an IP, the
columns provide the following infos:

**Date banned** - when you banned the comment's IP **IP** - the IP
**Name used** - What the user entered as his “name”. **Banned for** the
reason you banned an IP: the comment's number. If you click on the
linked number, the comment will be opened in edit mode for reviewing and
possibly editing. The last column provides an “unban” for the IP (Ip\#
in the second column).