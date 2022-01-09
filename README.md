# San Andreas State Template
## Version 1.9.22

The San Andreas State Template is an HTML template and website standard created by the California Department of Technology to state agencies and departments within the State of California and beyond. Please visit webstandards.ca.gov for more information.

This is a modified version of the template used to create internal websites for the State of San Andreas' Agencies within PJRP.

We encourage you to utilize GitHub to provide feedback and collaborate on the development of the next San Andreas State Template! For questions please email hmayotte@mdhholdings.org

________________________________________

Step 1 - Instructions
Extract the zip file to your web root directory (usually htdocs or wwwroot). Make sure your web server is configured to process SSI. It might be configured to process only files with certain file extensions such as .stm. In that case, you'll need to either name your pages with a .stm extension or configure your server to process .html as well.

________________________________________

Step 2 - Navigation Type
Select your navigation type. Megamenu, Dropdowns, or Single level and Open /ssi/navigation.html and update line 8.

________________________________________

Step 3 - Color Scheme
Select a color scheme and Open head_css_js.html and Update line 25.

________________________________________ 

Step 4 - Google Analytics
Open /ssi/analytics.html and Insert your Google Analytics ID at line 4.

________________________________________

Step 5 - Header Images
Replace the sample /images/template2014/header-organization.png with your own logo and organization name. Replace /images/template2014/(Color Scheme)/header-background.jpg with your own image.
If using the optional slideshow banner open /ssi/header-slideshow-banner.html and add your own images and captions. If NOT using the slideshow banner open index.html and delete the include reference on line 55. The reference code will be <!--#include virtual="/ssi/header-slideshow-banner.html" -->

________________________________________

Step 6 - Search Format
By default the search field is smaller and located in the upper right corner of the site. The primary page templates (often the homepage) can have a large "Featured Search Box" in the center of the header. To enable this format open any template and locate the <div id="head-search" class="search-container"> and add the .featured-search class in addition to the existing .search-container class

________________________________________

Step 7 - Search Engine
Create a search engine results page (SERP) or customize the sample serp.html. Open /ssi/search.html and enter your search engine ID at line 9 and line 21. Open serp.html and  enter your search engine ID at line 63. If you change the filename or location of your SERP, you'll need to update search.js, line 6, with your new path.

________________________________________

Step 8 - Page Templates
There are four (4) master template page layouts to choose from. A pages layout can be controlled by applying two (2) classes to the <body> element. By default pages will have the smaller banner area and single column. Adding a class of .primary will designate a page a landing page and use the taller header image. Adding a class of .two-column will add a sidebar on the right side of the page. You are free to mix and match .primary and .two-column classes to achieve the layout desired. For an inteactive demo please see the following sample page: /sample/page-templates.html

________________________________________

Step 9 - Icons (optional)
Replace the "favorites" icons with your own: /images/template2014/apple-touch-icon-*.png /favicon.ico

________________________________________ 

Step 10 - Content
The /sample/index.html file contains links to examples of the new content styles as well as documentation and code that can be copied.
* Accordion Lists
* Carousels & slideshows
* Countdowns
* Color Schemes
* Info/News blocks styles
* List styles
* Buttons styles
* Heading & parahraph styles
* Icon fonts
* Form styles
* Gallery
* Navigation Menus
* Number Counters
* Panes
* Progress blocks
* Sections
* Tables
* Tabs
* Useful content modules

________________________________________

Custom CSS (optional)
CSS and JS is included in the core by default. If a custom build is desired all source files can be compiled using open source tools. Gulp and Node are recommended. Compiling from source allows for a smaller build using only the components that are necessary.