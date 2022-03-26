AMF Theme
=========

Summary
-------
Acme Movie Fanatics (AMF) is developing an online community using Liferay Portal for its members.  Part of the initial phase is to redesign the look-and-feel of this community site.  AMF has hired a design firm to create this new look-and-feel for their site.  Now, they need this new design translated into a Liferay Portal theme.

Objective
---------
Create a new AMF theme based on the given design.

Requirements
------------
### Assumptions
* Initial set of content has been created (they are available via a LAR file for the AMF site which is provided).

### General Specifications
* Theme should have 2 color schemes (light & dark).
* Header should span across the entire width of the browser window.
* Content and footer should have fixed width.
* Header and footer both have navigation bars with different designs.
* The navigation bar on the header should be horizontal with a red background.
* The sign-in link should look like a button per the design screenshot.

### Technical Specifications
* Breadcrumb should be removed from theme (not simply hidden via CSS).
* The AMF logo should be included directly in the theme via the init_custom.vm file (so to not be alterable in the Control Panel UI).
* To keep our site performance at the highest level, custom CSS should be kept to 200 lines or less.
* Do **not** use ```!important``` with your CSS selectors.
* Remove portlet borders.
* Use Sass and Compass.
* Footer should be created in a new ```VM``` file.

### Design
#### Home Page ([full size] [1])
![home page](http://farm8.staticflickr.com/7418/13111094385_b25cd28416_z.jpg)
#### Upcoming Release ([full size] [2])
![coming soon](http://farm4.staticflickr.com/3827/13110803754_becbdd8717_z.jpg)
#### Light Color Scheme ([full size] [3])
![light color scheme](http://farm3.staticflickr.com/2156/13111185065_caab7436e2_z.jpg)
#### Trailer ([full size] [4])
![trailer](http://farm8.staticflickr.com/7319/13111324643_466a91caaa_z.jpg)

## Resources
The existing AMF site and all the related assets can be imported using the following [LAR file] [5].

####### components and features used
`html`, `css`, `theme`, `plugins-sdk`

[1]: http://farm8.staticflickr.com/7418/13111094385_b06f50103a_o.png
[2]: http://farm4.staticflickr.com/3827/13110803754_046514ebd7_o.png
[3]: http://farm3.staticflickr.com/2156/13111185065_f2a805f151_o.png
[4]: http://farm8.staticflickr.com/7319/13111324643_62daa215df_o.png
[5]: https://in.liferay.com/documents/210910/373495/Theme-Training-AMF-01-Public-Pages.lar/ee02e129-80d9-4b3d-adae-c8658133bbf4
