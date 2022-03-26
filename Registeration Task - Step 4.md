Registration Search
===================
Summary
-------
Acme Movie Fanatics (AMF) is developing an online community using Liferay Portal for its members.  The third phase of this project is to provide services to event coordinators.

Objective
---------
AMF would like to give some of their third-party event coordinators the ability to find AMF members in a specific area.  This would help them reach movie enthusiasts that can promote the health and participation of the AMF ecosystem.

Requirements
------------
### General Specification
* Third-party event coordinators (TEC) are not AMF staff members and should not have administrative access.
* Third-party event coordinators will be given the proper role which will allow them to view and use the features described in this project.
* Permission is needed to access this search feature.  TEC's role will be given this permission to perform the search.
* The TEC will be able to search users in a specific region by providing a 5-digit postal code.
* The feature should only search members' primary addresses.
* The list of search results (list of users) should display the following:
	* User's First Name and Last Initial
	* User's Screen Name
	* User's Email Address
* The search results should have a header that includes the 5-digit postal code like the following: `Search Results for 90210`.
* The search results should be paginated with the default of 5 users per page.

### Technical Requirement
* The input text field for entering the 5-digit postal code should be its own portlet.
* The display of search results should be its own (separate from the input) portlet.
* Use the 30/70 layout on the page.
* Place the search input portlet on the 30 column.
	* The search portlet should retain the postal code.
	* Input should be validated to be numeric and contains 5 digits.
	* Search should be done on database only, not search index.
* Place the search results portlet on the 70 column.
	* If there are no results to display, show the following message:

	```No results found.  Please try a different search criteria.```

* The portlets should employ the Inter-Portlet Communication feature of the portal.

### Wireframe
Below is a mock-up of the two portlets.
![Portlet Mock-ups](http://farm3.staticflickr.com/2806/9718539009_d878f31bef_z.jpg).

### UI
* Refer to the wireframe for general placement of the different UI elements.
* Use as much AUI and Liferay taglibs as possible.
* Use Liferay's pagination feature (which looks a bit different from wireframe).

### Non-Functional Requirements
* Module should following naming conventions found in training material and Liferay code base.
* Portlets must be named ```amf-search``` and ```amf-search-results```.
* Module must work in Liferay DXP (preferably the latest SP).

###### Components and Features Used
`Service Builder`, `Portlet`, `Accessing Liferay Core Services`, `Validation`, `Inter Portlet Communication (IPC)`, `AUI`, `Search Container`, `Custom Finder`, `SQL`, `Pagination`.
