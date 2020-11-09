## ATTRIBUTES OF SECTION TAG


### Syntax
```xml
        <b:section attribute="value">
            <!-- Widgets -->
            <!--Section --> 
        </b:section>
```

### Example

```xml
                <b:section class='header' id='header' maxwidgets='1' showaddelement='no'>
                   
                    <b:widget id='Header1' locked='true' title='' type='Header'></b:widget>


                </b:section>
```



<table class="tableizer-table"><thead>
<tr class="tableizer-firstrow"><th>Attributes </th><th>Values </th><th>Required/Optional </th><th>Refers to</th></tr>
</thead><tbody>
<tr><td>id </td><td>Unique name. Only letters and numbers are allowed. Example: header, navbar, sidebar, footer etc. </td><td>Required </td><td>Determining and customizing section with id.</td></tr>
<tr><td>class </td><td>Same as id. </td><td>Optional </td><td>Determining and customizing section with class.</td></tr>
<tr><td>maxwidgets </td><td>In numbers. Example: 1, 2, 3, 10 etc. </td><td>Optional </td><td>How much widgets we want to keep within this section.</td></tr>
<tr><td>showaddelement </td><td>Values of this are in Boolean. Yes and No. </td><td>Optional </td><td>If yes then the section will allow to add gadgets as widget, otherwise none.</td></tr>
<tr><td>growth </td><td>horizontal and vertical. </td><td>Optional </td><td>If vertical then section will be arranged side-by-side. Othewise stacked.</td></tr>
</tbody></table>