Acme Movie Fanatics
===================
Summary
-------
Acme Movie Fanatics (AMF) wants to build an online community for its members.  The site will consist of movie related content and also social features as well.

**NOTE**:

* This assignment can be completed in both Liferay version 7.0 and 7.1. When doing this project in Liferay 7.1 it may be necessary to use Liferay 7.0 documentation as well as 7.1 documentation. The documentation for Liferay 7.0 is currently more robust than the 7.1 documentation. That being said, most requirements are fulfilled similarly between the two versions of Liferay. One notable exception is how site pages are created.

* In order to setup and test email related functionality, please create ***all*** test users using the alias feature from your `liferay.com` email account.  For example, if your email address with Liferay is `joe.shmoe@liferay.com`, then you can create additional users by appending a `+` sign with an alphanumeric string between the `+` sign and the `@` sign.  Here is an example: `joe.shmoe+test01@liferay.com`.  Emails sent to that address will show up in your mailbox just like your real email address.  This allows you to create any number of test users with just your email address. You can configure Liferay to use your Google Apps email account as the email server or setup a [fake SMTP server](https://grow.liferay.com/share/Lightweight+SMTP+servers+for+testing+e-mail+notifications) to intercept the emails. If you are using a Google Apps email account as the email server you will have to enable 'less secure app access' for that Google account. Follow this link to do so: [Less Secure App Access](https://myaccount.google.com/lesssecureapps) 

Requirements
------------
### Site & Pages ###
* AMF would like to have an open guest community where non-logged in users can view all public content, including public forum posts and blogs.
* This guest site should have the following URL: amf.com
	* AMF does not want to see /web/guest in the URL.
	* Note that on your development machine, it is acceptable to keep using high number ports like 8080.
* The site should have the following pages:
	* Home - landing page with welcome message and short spiel about the site.
	* Blog - A page with blog posts from site content creators and editors.
	* Forums - A page with the Message Boards portlet.

### User & Role ###
- Make sure users cannot use the email address admin@AMF.com.

#### AMF Members ####
* AMF members signing up for an account should inherit the `User` role **only** (no `Power User` role should be given).
* Disable the Terms of Use when a user signs up for an account.
* In addition to the default `User` permissions, AMF members should also have the following and nothing more:
	* Message Boards:
		* Add Message (any where)
		* View
		* Reply to Message
		* Update their own Message (Not Category)
		* Subscribe
		
#### AMF Staff ####
* AMF Staff should all have the `Power User` role.
* Content Creator - a role that allows AMF staff to create content for the site.  However, these users can **not** approve/publish content.
* Content Editor - a role that allows AMF staff to approve/publish content.
* Site Editor - a role that allows AMF staff to:
	* add, remove, or rearrange portlets on the site
	* change layouts
	* add, remove site pages
* Forum Administrator - a role that allows AMF staff to Manage Message Boards.  This role should be given all permission related to Message Boards.

#### Admins ####
* Omni-Admin should be given to just one user account with email `admin@liferay.com`.
* `test@liferay.com` account should be removed or changed.

### Authentication ###
* Users should login with their email address
* Allow user to reset password via email link.
* New users must verify their email addresses via email link.

### Organization & User Group ###
#### Movie Awards Organization ####
* If using Liferay 7.1, define a new type of organization through **System Settings** in the **Users** category. If using Liferay 7.0 you'll have to define a new type of organization using **portal-ext.properties**:
	* Type: custom-organization.
	* Top level
	* Suborganizations can only be of type regular-organization.
* Create a **custom** non searchable **field** "nickname" with value: "Oscar Guys" for the organization. Make sure a user can view and update this field.

#### Movie Club User Group ####
- Event Creator - a role that allows members of the user group to create events in the calendar portlet (deployed on the home page for the AMF site).
- Should contain one user from each of the following types:
	- AMF staff
	- AMF member
	- User that belongs to the Movie Awards Organization
- The rest of users should not belong to this user group.

### Instance Settings ###
* Site should use Eastern Standard Time as its default timezone.
* Language should be limited to English at this point.
* Change the portal logo to one of your choice.

### Message Boards ###
* Create the following public categories that all users (including guest) can view:
	* New Theatrical Releases
	* New DVD Releases
	* Home Theatre System
	* New Movie Ideas
* Create a Staff only category that only AMF Staff can View.

### Blog ###
* Only Content Creators and Editors can create blog entries.
* Anyone can view the Blog page and blog entries.

### Password Policies ###
- Create a new Password Policy with the following password properties:
	- It must be changeable but not require a change when the user first logs in.
	- Users assigned to it cannot reuse the same password.
	- It should expire in 4 weeks and display a warning two days before expiration.
	- It should lock the account if a user tries to log in unsuccessfully 4 times in 5 minutes, and only the administrator can unlock the account.
- Assign all members in the Movie Awards organization to this password policy
