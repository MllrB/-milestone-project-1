# OfficePrinters

Code Institute - Milestone Project 1 - User Centric Front End Development

This website is intended to generate sales leads for printers in the B2B environment. The concept is proven as there is already a live website that achieves leads, however, the live site has been performing poorly of late and I felt that this could be greatly improved with a more enticing look and feel and more focused design structure.

* [Existing Live Site](http://www.officeprinters.ie)
* [My Re-Designed Site](https://mllrb.github.io/OfficePrinters/)


## UX
---------

The primary goal of the site is for the customer to request a quotation.

### User Stories

##### The Site owner 
* As the site owner, I want to advertise my business in order to attract new business customers
* As the site owner, I want to provide a way for new customers to contact me to initiate the purchase of a new printer
* As the site owner I want to direct all users, business or home users, to visit my existing ecommerce shop in order to purchase printer consumables

##### The Customer 
* As a customer, I want to get a quotation on a new printer for my office
* As a customer, I want to reduce the workload involved in researching and choosing a new printer
* As a customer I want to some information on the product or service provided by the company


### Design Considerations
The website is targeted towards a corporate audience with an emphasis on reducing the user’s workload. With this in mind, my goal was to design the site to be professional in look and have a clean, uncluttered and relaxing feel. To achieve this I chose soft colours and clear, easily legible fonts.

My intuition was that most business user’s would be researching new printers by browsing on a computer as opposed to a mobile device so I decided to separate the site’s features over 5 pages. Also, despite being the main focus for the site, I did not want to confront the user with a form to fill out on the landing page.  I wanted to point the user towards requesting a quote at every opportunity while still allowing the user to come to that decision at a time of their choosing.

I felt that a multi-page design was most suited to incorporating the following needs:

##### Needs of the Site Owner 
* Contact Form: A short form with the customer's contact information and basic information on the customer's requirements. This is the most important feature of the website and all pages have a link to it.
* A product page showcasing a few products the owner can provide and the brands the owner can source.
* Information about the company and links to the sister site.

##### Needs of the customer
* A means to obtain a quotation
* Easily accessible contact information
* Some information about the company
* Some information on the products the company provides

### Wireframes

[Site Wireframes](/OfficePrinters/docs/officeprinters_Wireframes.pdf)

##### Navigation
I had initially intended the following navigation structure, however, with the nav bar displayed on every page, there was no need to try to implement it as it is possible to navigate to all pages from any page.

![Initially Intended Navigation Structure](/OfficePrinters/assets/media/navigation-structure.png)


## Features
---------

### Existing Features
1. A landing page directing users to a contact form with a view to getting a quotation for a printer. The landing page also features a snapshot of the products page and a link to a sister site which offers printer consumables.

1. A short contact form allowing users to request a quotation by filling in some basic information about themselves and their requirements.

1. A product page showcasing a couple of the products on offer and the brands available to the company. Each product has a logo, an image, some quick benefits to the product and a link to more information. There is also a request a quote button which opens a modal asking for contact information. I intend for this to alert the site owner to the customer's interest in a particular product although this feature is not functional at present.

1. An About Us page displaying some information about the company and a map showing where the company is situated 

1. A contact page showing users the address, telephone number, email address and opening hours for the company. All are clickable. The address links to a pin on google maps, the phone number initiates a call if applicable (on mobile), the email address will open a mail client.

### Features for the Future
1. Implentation of an plugin that will email the site owner with customer details and requirements when a quotation is requested
1. Modal thanking the customer for submitting their quotation request

## Technologies Used
---------
* HTML
* CSS
* Bootstrap 4.4.1

## Testing
---------

I tried to achieve the owner's user stories brief by:
* providing information on the company on the about us page and also by showing the brands available and some sample products
* providing contact information for the company and by providing a form for a customer to fill in order to request a quotation. There are links to this form on most of the pages on the website and on the product examples page, the "Request a Quote" button has a shortened version of the form with the intention of allowing the customer to declare their interest in that particular product.
* providing links and information to the company's sister site on multiple relevant pages.

In terms of the customer user stories, I met the brief by:
* providing a form to fill in to request a quotation.
* ensuring that the form is short with the only required information being the customer's contact details. 
* providing information in the about us page, the brands available to source and some sample products.

I have manually tested all the links on the site and all are successful. All external links ore set to open in a new tab using target="blank". All internal links work as required and the links from the landing page to the product page go directly to the product associated with that link (i.e. the Epson link centers on the Epson product and the OKI link centers on the OKI product).

As intended, the contact form rejects entries if any of the required fields (company name, contact name, email address and contact phone number) are left bank. In addition, invalid email addresses and phone numbers with less than 7 digits are also rejected. If all fields are valid, the page refreshes. This is true for the form on the Get a Quote page and also for the modals launched via the products page.

I used Chrome and Chrome developer tools to test layout and responsiveness and once I was happy with this I further tested accross multiple browsers - Chrome, Firefox, Edge, Safari and Opera. For mobile devices I tested on an iPhone, a Huawei android phone and also a Samsung Galaxy. I don't have access to a tablet size device so had to rely on Chrome developer tools to test this screen size. I encountered some issues with overflow on the right side of mobile devices. To counteract this I needed to use a wrapper around all the content on each page with the overflow-x set to hidden. There is still overflow on the Microsoft Edge browser although I think this is to do with additional navigation functionality on the browser itself.


I validated my CSS and HTML using [jigsaw.w3.org/](https://jigsaw.w3.org/css-validator/) and [validator.w3.org/](https://validator.w3.org/).   All tests passed except:

CSS: 
* -webkit-transition is an unknown vendor extension
* -moz-transition is an unknown vendor extension
* -o-transition is an unknown vendor extension

Solution: Non-critical, ignored

HTML:
*  Bad value 100% for attribute width on element iframe: Expected a digit but saw % instead.

Solution: Value of 100% is necessary to fill the div, ignored


## Deployment
----------

To deploy this site,  I opened my GitHub repository and selected "Settings". From there I scolled down to the GitHub Pages section and selected the source as my Master Branch.

* Git Repository: https://github.com/MllrB/OfficePrinters
* URL:  `https://mllrb.github.io/OfficePrinters/ `	
* Link: [OfficePrinters](https://mllrb.github.io/OfficePrinters/)

#### To run locally...
**Either** clone this repository by running the command `git clone https://github.com/MllrB/OfficePrinters.git` in your terminal.

**Or** open using GitPod by clicking the GitPod button to the right of this repository 

## Credits
---------

### Content

* All text on the site was written by me.
* Icons provided by [FontAwesome](https://fontawesome.com/)
* Fonts provided by [Google Fonts](https://fonts.google.com/)
* Maps provided by [Google Maps](https://goo.gl/maps/3MoyscgQnwBb2USa6)

### Media
* Landing page photo downloaded from [Canva](https://www.canva.com/), photo by Mali Maeder
* Footer background photo downloaded from [Canva](https://www.canva.com/), photo by Matthias Zomer
* Brand logos downloaded from [brandsoftheworld.com](https://www.brandsoftheworld.com/)
* Printer images courtesy of Epson Neon and OKI PartnerNet (both partner portals)

### Acknowledgements

* Solution to how to style bootstrap inputs from [igaster](https://stackoverflow.com/users/1680535/igaster)  :  [(Solution)](https://stackoverflow.com/questions/14820952/change-bootstrap-input-focus-blue-glow)
* Solution to how to style bootstrap radio buttons and checkboxes from [webdevbooster](https://stackoverflow.com/users/8270343/webdevbooster)  :  [(Solution)](https://stackoverflow.com/questions/48401587/bootstrap4-radio-button-background-and-fill-color)
* Resources used: [Bootstrap Documentation](https://getbootstrap.com/docs/4.4/getting-started/introduction/) nd [CSSTricks](https://css-tricks.com/)







