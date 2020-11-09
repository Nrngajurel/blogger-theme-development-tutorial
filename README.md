# Blogger Theme Development Tutorial



# Getting Start

### Starter Template
```xml
<?xml version="1.0" encoding="UTF-8" ?>
     <!DOCTYPE html>
     <html lang='en-US' xmlns='http://www.w3.org/1999/xhtml' xmlns:b='http://www.google.com/2005/gml/b' xmlns:data='http://www.google.com/2005/gml/data' xmlns:expr='http://www.google.com/2005/gml/expr' xmlns:og='http://ogp.me/ns#'>
<!--
    xmlns:b – ‘b’ specifies that this namespace is used to access the blogger elements.
    xmlns:data – It is used to specify that from where the data of the blog comes.
    xmlns:expr – Calculates the expression for attributes.
-->
<head>
        <b:include data='blog' name='all-head-content' />
        <title>
            <data:blog.pageTitle/>
        </title>
        <meta content='width=device-width, initial-scale=1' name='viewport' />
        
        <b:skin>
            <![CDATA[  
            /* Custom CSS code goes here... */
            ]]>
        </b:skin>
    </head>
    <body>
        <div id="blog-wrapper">
            <header>
                <b:section class='header' id='header' maxwidgets='1' showaddelement='no'>
                    <b:widget id='Header1' locked='true' title='' type='Header'></b:widget>
                </b:section>
            </header>
            <div id="content-wrapper">
                <div class="content-table">
                    <div class="content-row">
                        <b:section class='main column' id='main' showaddelement='yes'>
                            <b:widget id='Blog1' locked='true' title='Blog Posts Section' type='Blog' />
                        </b:section>
                        <aside class="column">
                            <b:section class='sidebar' id='sidebar' maxwidgets='' showaddelement='yes'>
                            </b:section>
                        </aside>
                    <div>
                </div>
            </div>
            <footer>
                <div>
                    Copyright © 2020 <strong><data:blog.title/></strong>
                </div>
            </footer>
         </div>
            </div>

        </div>

    </body>
    </html>

```

<table class="tableizer-table"><thead>
<tr class="tableizer-firstrow"><th>Blogger Data Tags </th><th>What Show</th></tr>
</thead><tbody>
<tr><td><code>&lt;data:post.dateHeader/&gt;</code></td><td>The post's date as header.</td></tr>
<tr><td><code>&lt;data:title/&gt;</code></td><td>The blog's title.</td></tr>
<tr><td><code>&lt;data:description/&gt;</code></td><td>The blog's description.</td></tr>
<tr><td><code>&lt;data:olderPageTitle/&gt;</code></td><td>Title of the older page of posts.</td></tr>
<tr><td><code>&lt;data:newerPageTitle/&gt;</code></td><td>Title of the newer page of posts.</td></tr>
<tr><td><code>&lt;data:commentLabel/&gt;</code></td><td>Number of Comments.</td></tr>
<tr><td><code>&lt;data:authorLabel/&gt;</code></td><td>It will show "posted by".</td></tr>
<tr><td><code>&lt;data:post.title /&gt;</code></td><td>The post's title.</td></tr>
<tr><td><code>&lt;data:post.body/&gt;</code></td><td>The post's content.</td></tr>
<tr><td><code>&lt;data:post.author/&gt;</code></td><td>The post's author name.</td></tr>
<tr><td><code>&lt;data:post.url/&gt;</code></td><td>The post' url link.</td></tr>
<tr><td><code>&lt;data:post.timestamp/&gt;</code></td><td>The post's date and time.</td></tr>
<tr><td><code>&lt;data:label.name/&gt;</code></td><td>The post's label.</td></tr>
</tbody>

</table>




<table class="tableizer-table"><thead>
<tr class="tableizer-firstrow"><th>Dynamic Anchor URL</th><th>What Show</th></tr>
</thead><tbody>
<tr><td><code>&lt;a expr:href='data:blog.homepageUrl &gt;Homepage&lt;/a&gt;</code></td><td>A text with homepage’s URL</td></tr>
<tr><td><code>&lt;a expr:href='data:post.url'&gt;Read More&lt;/a&gt;</code></td><td>Read More Text with Post’s URL</td></tr>
<tr><td><code>&lt;a expr:href='data:label.url' property='v:title' rel='v:url'&gt;&lt;data:label.name/&gt;&lt;/a&gt;</code></td><td>Label Name with Label’s URL</td></tr>
<tr><td><code>&lt;a expr:href='data:post.newerLinkUrl'&gt;&lt;data:post.newerLinkText/&gt;&lt;/a&gt;</code></td><td>Newer Post Text with Newer Post URL</td></tr>
<tr><td><code>&lt;a expr:href='data:post.olderLinkUrl'&gt;&lt;data:post.newerLinkText/&gt;&lt;/a&gt;</code></td><td>Older Post Text with Older Post URL</td></tr>
<tr><td><code>&lt;a expr:href='data:comment.authorUrl' rel='nofollow'&gt;&lt;data:comment.author/&gt;&lt;/a&gt;</code></td><td>Author’s name with URL</td></tr>
<tr><td><code>&lt;a expr:href='data:comment.url' title='comment permalink'&gt;&lt;data:comment.timestamp/&gt;&lt;/a&gt;</code></td><td>Comment Text to comment with URL</td></tr>
</tbody></table>