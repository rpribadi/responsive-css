Responsive CSS
==============

Common css classes for responsive design (adopted from [Twitter Bootstrap](http://twitter.github.io/bootstrap/scaffolding.html#responsive)).

Usage
-----

Simply include <code>responsive.css</code> to your HTML file

```html
<html>
    <head>
        <link href="/static/css/responsive.css" rel="stylesheet">
	    <link href="/static/css/your_style.css" rel="stylesheet">
    </head>
    <body>
        .
        .
    </body>
</body>
```

### Example 1

```html
<p class='visible-large-screen'>Only visible for large screen</p>
<p class='visible-tablet-landscape'>Only visible for tablet landscape</p>
<p class='visible-tablet-portrait'>Only visible for tablet portrait</p>
<p class='visible-phone-landscape'>Only visible for phone landscape</p>
<p class='visible-phone-portrait'>Only visible for phone portrait</p>
```

### Example 2

```html
<table>
    <tr>
        <th>Col 1</th>
        <th class='hidden-below-phone-landscape'>Col 2</th>
        <th class='hidden-below-tablet-portrait'>Col 3</th>
        <th class='hidden-below-tablet-landscape'>Col 4</th>
        <th class='hidden-below-large-screen'>Col 5</th>
    </tr>
    <tr>
        <td>Always Visible</td>
        <td class='hidden-below-phone-landscape'>Hidden Below Phone Landscape</td>
        <td class='hidden-below-tablet-portrait'>Hidden Below Table Portrait</td>
        <td class='hidden-below-tablet-landscape'>Hidden Below Tablet Landscape</td>
        <td class='hidden-below-large-screen'>Hidden Below Large Screen</td>
    <tr>
</table>
```

### Example 3

```html
<div class='hidden-below-tablet-portrait'>
    <p>Visible for large screen, tablet landscape & tablet portrait.</p>
</div>
<div class='visible-below-tablet-portrait'>
    <p>Visible for phone landscape & phone portrait.</p>
</div>
```

Available Classes
-----------------

    .visible-large-screen
    .visible-tablet-landscape
    .visible-tablet-portrait
    .visible-phone-landscape
    .visible-phone-portrait
    
    .visible-below-large-screen
    .visible-below-tablet-landscape
    .visible-below-tablet-portrait
    .visible-below-phone-landscape

    .hidden-large-screen
    .hidden-tablet-landscape
    .hidden-tablet-portrait
    .hidden-phone-landscape
    .hidden-phone-portrait

    .hidden-below-large-screen
    .hidden-below-tablet-landscape
    .hidden-below-tablet-portrait
    .hidden-below-phone-landscape

Screen Size Category Definition
-------------------------------

* Large Screen
    > min-width: 1200px

* Tablet Landscape <br />
    > max-width: 1199px<br />
    > min-width: 980px

* Tablet Portrait<br />
    > max-width: 979px<br />
    > min-width: 768px

* Phone Landscape<br />
    > max-width: 767px<br />
    > min-width: 481px<br />

* Phone Portrait<br />
    > max-width: 480px

Mobile Device Test Result
-------------------------

Mobile Device           |Landscape Mode     |Portrait Mode
------------------------|-------------------|-------------
iPad2                   |Tablet Landscape   |Tablet Portrait
Samsung Galaxy Tab      |Phone Landscape    |Phone Portrait
Samsung Galaxy Tab 2    |Tablet Landscape   |Phone Landscape
iPhone4                 |Phone Portrait     |Phone Portrait
iPhone5                 |Phone Landscape    |Phone Portrait
Samsung Galaxy SIII     |Phone Landscape    |Phone Portrait
Samsung Galaxy SIV      |Phone Landscape    |Phone Portrait
Samsung Galaxy Note II  |Phone Landscape    |Phone Portrait


<code>visible-*</code> Classes
------------------------------

These classes will set elements to be displayed only for 1 specific screen type.

|                      | .visible-large-screen | .visible-tablet-landscape | .visible-tablet-portrait | .visible-phone-landscape | .visible-phone-portrait |
| -------------------- | :-------------------: | :-----------------------: | :----------------------: | :----------------------: | :---------------------: |
| **Large Screen**     | **Visible**           | Hidden                    | Hidden                   | Hidden                   | Hidden                  |
| **Tablet Landscape** | Hidden                | **Visible**               | Hidden                   | Hidden                   | Hidden                  |
| **Tablet Portrait**  | Hidden                | Hidden                    | **Visible**              | Hidden                   | Hidden                  |
| **Phone Landscape**  | Hidden	               | Hidden                    | Hidden                   | **Visible**              | Hidden                  |
| **Phone Portrait**   | Hidden		           | Hidden                    | Hidden                   | Hidden                   | **Visible**             |


<code>visible-below-*</code> Classes
------------------------------

These classes will set elements to be displayed for a range of screen types.

|                      | .visible-below-large-screen | .visible-below-tablet-landscape | .visible-below-tablet-portrait | .visible-below-phone-landscape |
| -------------------- | :-------------------------: | :-----------------------------: | :----------------------------: | :----------------------------: |
| **Large Screen**     | Hidden                      | Hidden                          | Hidden                         | Hidden                         |
| **Tablet Landscape** | **Visible**                 | Hidden                          | Hidden                         | Hidden                         |
| **Tablet Portrait**  | **Visible**                 | **Visible**                     | Hidden                         | Hidden                         |
| **Phone Landscape**  | **Visible**                 | **Visible**                     | **Visible**                    | Hidden                         |
| **Phone Portrait**   | **Visible**    	         | **Visible**                     | **Visible**                    | **Visible**                    |

* <code>.visible-below-large-screen</code> is equal to <code>.hidden-large-screen</code><br />
* <code>.visible-below-phone-landscape</code> is equal to <code>.visible-phone-portrait</code>

<code>hidden-*</code> Classes
-----------------------------

These classes will set elements to be hidden only for 1 specific screen type.

|                      | .hidden-large-screen | .hidden-tablet-landscape | .hidden-tablet-portrait | .hidden-phone-landscape | .hidden-phone-portrait |
| -------------------- | :------------------: | :----------------------: | :---------------------: | :---------------------: | :--------------------: |
| **Large Screen**     | **Hidden**           | Visible                  | Visible                 | Visible                 | Visible                |
| **Tablet Landscape** | Visible              | **Hidden**               | Visible                 | Visible                 | Visible                |
| **Tablet Portrait**  | Visible              | Visible                  | **Hidden**              | Visible                 | Visible                |
| **Phone Landscape**  | Visible              | Visible                  | Visible                 | **Hidden**              | Visible                |
| **Phone Portrait**   | Visible	          | Visible                  | Visible                 | Visible                 | **Hidden**             |


<code>hidden-below-*</code> Classes
-----------------------------

These classes will set elements to be hidden for a range of screen types.

|                      | .hidden-below-large-screen | .hidden-below-tablet-landscape | .hidden-below-tablet-portrait | .hidden-below-phone-landscape |
| -------------------- | :------------------------: | :----------------------------: | :---------------------------: | :---------------------------: |
| **Large Screen**     | Visible                    | Visible                        | Visible                       | Visible                       |
| **Tablet Landscape** | **Hidden**                 | Visible                        | Visible                       | Visible                       |
| **Tablet Portrait**  | **Hidden**                 | **Hidden**                     | Visible                       | Visible                       |
| **Phone Landscape**  | **Hidden**                 | **Hidden**                     | **Hidden**                    | Visible                       |
| **Phone Portrait**   | **Hidden**		            | **Hidden**                     | **Hidden**                    | **Hidden**                    |

* <code>.hidden-below-large-screen</code> is equal to <code>.visible-large-screen</code><br />
* <code>.hidden-below-phone-landscape</code> is equal to <code>.hidden-phone-portrait</code>


Author
------

Riki Pribadi
+ https://github.com/rpribadi
+ https://twitter.com/flakeware

Questions?
----------

If you have any questions, please feel free to contact the author.
