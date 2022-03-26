Stanley Theme
=============

Summary
-------
To show that you have a good grasp of HTML and CSS, it is now time to create a Liferay theme. Following the documentation provided by Liferay, create the Stanley theme.

Objective
---------
Create a new theme based on the given design.

Requirements
------------
### Assumptions
* Initial set of content has been created (they are available via a LAR file for the AMF site which is provided).

### General Specifications

* Header should span across the entire width of the browser window.
* Theme parent should be ```_styled```
* Header and footer both have navigation bars with different designs.
* The sign-in link should look like a button per the design screenshot.

### Technical Specifications
* Breadcrumb should be removed from theme (not simply hidden via CSS).
* To keep our site performance at the highest level, custom CSS should be kept to 300 lines or less.
* Do **not** use ```!important``` with your CSS selectors.
* Remove portlet borders via the look and feel xml file.
* Use Sass and Compass for CSS3 effects.
* Create a responsive navigation.
* Follow the Liferay best practices for [CSS] [1] and [JS] [2].

### Design
#### About Stanley (Desktop) ([full size] [3])
![home page](https://farm3.staticflickr.com/2925/14329969301_92ffd0eafa_z.jpg)
#### About Stanley (Mobile) ([full size] [4])
![home page mobile](https://farm6.staticflickr.com/5315/14333305835_66e7d0ccea.jpg)
#### Blogs (Desktop) ([full size] [5])
![work](https://farm4.staticflickr.com/3919/14333305825_30ab239772_z.jpg)
#### Blogs (Mobile) ([full size] [6])
![work mobile](https://farm6.staticflickr.com/5521/14331587442_b86489bdc9.jpg)
#### Contact (Desktop) ([full size] [7])
![about](https://farm4.staticflickr.com/3866/14310168536_00233c80ff_z.jpg)
#### Contact (Mobile) ([full size] [8])
![about mobile](https://farm6.staticflickr.com/5521/14329969171_f60a1a9427_z.jpg)
#### Home (Desktop) ([full size] [9])
![blog](https://farm4.staticflickr.com/3868/14310168506_a3e4803c70_z.jpg)
#### Home (Mobile) ([full size] [10])
![blog mobile](https://farm3.staticflickr.com/2922/14331587222_8dc2efb390.jpg)
#### Work (Desktop) ([full size] [11])
![contact](https://farm4.staticflickr.com/3841/14332578324_ed683987e5_z.jpg)
#### Work (Mobile) ([full size] [12])
![contact mobile](https://farm6.staticflickr.com/5555/14146640909_fc2099b8c6.jpg)

## Resources
The assets seen in the screenshots can be imported using the following [LAR file] [13].  Theme development is covered in our public training.  You can find the material on [liferay.com/group/training][14].  A quick start guide can also be found [here][15].

####### components and features used
`html`, `css`, `theme`, `plugins-sdk`


[1]: https://in.liferay.com/web/global.engineering/wiki/-/wiki/Core+Development+Main/Peer+Reviews+Checklist#section-Peer+Reviews+Checklist-CSS
[2]: https://in.liferay.com/web/global.engineering/wiki/-/wiki/Core+Development+Main/Peer+Reviews+Checklist#section-Peer+Reviews+Checklist-JavaScript
[3]: https://farm3.staticflickr.com/2925/14329969301_0dc50a6de1_o.png
[4]: https://farm6.staticflickr.com/5315/14333305835_7bcfcbfe77_o.png
[5]: https://farm4.staticflickr.com/3919/14333305825_a76a367ac5_o.png
[6]: https://farm6.staticflickr.com/5521/14331587442_68937e72aa_o.png
[7]: https://farm4.staticflickr.com/3866/14310168536_20840c081e_o.png
[8]: https://farm6.staticflickr.com/5521/14329969171_2a877a297e_o.png
[9]: https://farm4.staticflickr.com/3868/14310168506_875d149444_o.png
[10]: https://farm3.staticflickr.com/2922/14331587222_decdfe7ae5_o.png
[11]: https://farm4.staticflickr.com/3841/14332578324_953337f01c_o.png
[12]: https://farm6.staticflickr.com/5555/14146640909_d731d461cd_o.png
[13]: https://in.liferay.com/documents/210910/373495/Theme-Training-Stanley-01-Public-Pages.lar/8767cb4b-326d-48d8-9857-05e08ac783bc
[14]: https://www.liferay.com/group/training/6.2/themes
[15]: https://www.liferay.com/documentation/liferay-portal/6.2/development/-/ai/creating-liferay-themes-liferay-portal-6-2-dev-guide-09-en
