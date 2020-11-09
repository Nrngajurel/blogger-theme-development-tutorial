#widgets

## Widgets Syntax
```xml
     <b:widget attribute='value'></b:widget>

```
<table class="tableizer-table"><thead>
<tr class="tableizer-firstrow"><th>Attributes </th><th>Values </th><th>Required/Optional </th><th>Refers to</th></tr>
</thead><tbody>
<tr><td>id </td><td>Unique name. Only letters and numbers are allowed. Example: header, navbar, sidebar, footer etc. </td><td>Required </td><td>Determining and customizing section with id.</td></tr>
<tr><td>type </td><td>Header, Blog, Profile, PageList, AdSense, Attribution, HTML </td><td>Required </td><td>Define the type of widget.</td></tr>
<tr><td>locked </td><td>yes, no </td><td>Optional </td><td>If yes then you can't delete or move this widget.</td></tr>
<tr><td>title </td><td>Put any title name. Example: Tools, Advertisement, Lists etc. </td><td>Optional </td><td>Show the title of this widget.</td></tr>
<tr><td>pageType </td><td>all, archive, main, item, static, all </td><td>Optional </td><td>Define the page type of widget.</td></tr>
<tr><td>mobile </td><td>yes, no, default </td><td>Optional </td><td>If yes, then the widget will be shown on mobile device.</td></tr>
</tbody></table>

### Examples

 #### Simple Example
 ```xml
       <b:widget id='Header1' locked='true' title='' type='Header'></b:widget> 
``` 


### nav menu
```xml
          <b:widget id='LinkList210' locked='true' title='Menu' type='LinkList' version='1'>
            <b:widget-settings>
              <b:widget-setting name='text-9'>Documentation</b:widget-setting>
              <b:widget-setting name='link-9'>#</b:widget-setting>
              <b:widget-setting name='text-8'>Seo Services</b:widget-setting>
              <b:widget-setting name='link-7'>#</b:widget-setting>
              <b:widget-setting name='text-10'>Download</b:widget-setting>
              <b:widget-setting name='link-3'>#</b:widget-setting>
              <b:widget-setting name='link-4'>#</b:widget-setting>
              <b:widget-setting name='text-1'>_Multi DropDown</b:widget-setting>
              <b:widget-setting name='text-0'>Features</b:widget-setting>
              <b:widget-setting name='text-3'>__DropDown 2</b:widget-setting>
              <b:widget-setting name='text-2'>__DropDown 1</b:widget-setting>
              <b:widget-setting name='text-5'>_ShortCodes</b:widget-setting>
              <b:widget-setting name='text-4'>__DropDown 3</b:widget-setting>
              <b:widget-setting name='text-7'>_Error Page</b:widget-setting>
              <b:widget-setting name='text-6'>_SiteMap</b:widget-setting>
              <b:widget-setting name='sorting'>NONE</b:widget-setting>
              <b:widget-setting name='link-1'>#</b:widget-setting>
              <b:widget-setting name='link-2'>#</b:widget-setting>
              <b:widget-setting name='link-0'>#</b:widget-setting>
              <b:widget-setting name='link-10'>#</b:widget-setting>
            </b:widget-settings>
            <b:includable id='main'>
            <div class='widget-content'>
              <ul itemscope='' itemtype='http://schema.org/SiteNavigationElement'> 
                <b:loop values='data:links' var='link'>
                  <li itemprop='name'><a expr:href='data:link.target' itemprop='url'><data:link.name/></a></li>
                </b:loop>
              </ul>

            </div>
          </b:includable>
          </b:widget>

```




