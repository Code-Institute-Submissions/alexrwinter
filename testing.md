# Testing

## Code testing
[W3C Markup Validation Service](https://validator.w3.org/) was used to test the validity of the HTML code.
[W3C CSS jigsaw validation service](https://jigsaw.w3.org/css-validator/) was used to test the validity of the CSS code.


## Browser Compatibility testing
The web page was opened in [Mozilla Firefox](https://www.mozilla.org/en-US/firefox/download/thanks/), [Google Chrome](https://www.google.com/chrome/), [Safari](https://www.apple.com/uk/safari/) and [Microsoft Edge](https://www.microsoft.com/en-us/edge): all functional.

## Manual testing

**General font sizing, margins, padding and content visibility, plus responsive specific elements and features (listed below) to be checked at all sizes & breakpoints. Checked in four ways:**
    
1.	Via Google Chrome’s ‘inspect’ feature (motoG4, Galaxy S5, Pixel2 Pixel2sl, iPhone 5/SE, iPhone 6/7/8, iPhone 6/7/8 Plus, iPhone X, iPad, iPad Pro ) and the ‘responsive’ setting which allows horizontal and vertical resizing of the viewport.

2.	By viewing and manually checking the website on my mobile, tablet and desktop devices.

3.	By opening the page in Firefox, Chrome, Edge & Safari (most used web browsers) on different devices.

4.  By asking users to visit the site and report any problems.

    
_**Details below itemise elements and features to be tested with expected outcome, followed by a PASS or FAIL statement. Where an issue has been found, solution is stated after the 'FAIL' with a correction of 'PASS' if appropriate.**_

-------------------------------------------------------------------------------------------------------------------
### Body
i. **Layout** no gaps at the edges of the page __PASS__

ii. **Text and formatting** everything aligned correctly, font sizing consistent, styling consistent, chosen fonts working correctly and easy to read __PASS__

### Landing Page
i.**Chevron** correctly aligned on all devices; when clicked, takes user to ‘about’ section: __PASS__ 

ii.**Contact button** takes user to ‘contact section’; correctly aligned, text responsive sizing: __PASS__ 

iii.**IMDb button** visible on all devices; when clicked takes user to personal IMDb page in a seperate tab: __PASS__ 

iv.**Text visibility** text not obscured by background image; easy to read on all devices: __PASS__ 

v.**Text animation** works on all devices, cross-browser, and appropriate timing to read information as it appears: __PASS__ 

vi.**Font sizing** responsive: __PASS__ 

### Navigation Bar
i.**Position**  right hand side on medium and large devices; centred at top of screen on mobile devices; aligned with landing page chevron in both cases: __PASS__ 

ii.**Collapsible** collapsible nav functions for mobile devices: __PASS__ 

iii.**Doesn’t obscure content**  spacing appropriate to not interact with website content: __PASS__ 

iv.**‘Scrollspy’** highlights current section across devices, background changes colour from dark to light green as user scrolls to each section: __PASS__ 

v.**Navigation links**  all links functional, IMDb link opens a new tab to personal IMDb page; links highlighted when clicked: __PASS__

vi.**Margins** spacing around text appropriate: __PASS__ 

vii.**Font sizing** responsive, clear to read: __PASS__ 

### About
i.**Alex photo**  button functionality & animation; moves from right hand size to bottom of section; ;hidden on mobile devices; image darkens when hovered; when clicked, takes user to personal IMDb page: __PASS__ 

ii.**‘Read more’ button** appears on medium and small devices where second paragraph is hidden; when clicked, it expands the second paragraph; changes colour from dark to light green when hovered or clicked: __PASS__ 

iii. **‘Let’s work together’ button** visible on large devices and obscured along with paragraph on medium and small devices; appears when ‘read more’ is clicked; when clicked, takes the user to the contact section of the website; colour change when hovered or clicked from dark to light green: __PASS__ 

iv.	**Paragraph sizes** responsive; inline 'get in in touch' link is bold and takes user to contact page':__PASS__ 

v. **Font sizing** responsive, clear to read:__PASS__ 

vi.	**Margins** responsive and appropriate to screen size: __PASS__ 


### Services
i. **Layout** responsive from horizontal on large screens to vertical on small screens: __PASS__ 

ii. **Font sizing** responsive, clear to read: __PASS__ 

iii. **Margins** responsive and appropriate to screen size: __PASS__ 


### Projects
i.	**Images** responsive sizing, changes from stacked layout on mobiles to two column layout on medium and large screens:__PASS__ 

ii.	**Images as buttons** each takes user to the relevant film page on IMDb in a seperate tab: __PASS__ 

iii. **Images animation** images 'light up' when hovered or clicked: __PASS__ 

iv.	**Margins** responsive and appropriate to screen size: __PASS__ 

v. **Font sizing** responsive, clear to read:  __PASS__ 

vi. **Expand '...' button** works to open and collapse extra content, changes color from light to dark when cliked or hovered: __PASS__ 


### Testimonials
i. **Logos for production companies** appropriate sizing, visibility, margins, etc: __PASS__ 

ii.	**Responsive layout** changes from horizontal layout on medium and large screens to vertical layout on mobile devices: __PASS__ 

iii. **Font sizing** responsive, clear to read: __PASS__ 

iv.	**Margins** responsive and appropriate to screen size: __PASS__

v. **Read more button** works to expand and collapse extra content: __PASS__


### Contact
i. **Title** font sizing appropriate, margins appropriate, text is centered and aligned correctly: __PASS__ 

ii.	**Contact form**
a. responsive sizing __PASS__ 
b. margins responsive  __PASS__ 
c. functionality- required fields working __PASS__ 

iii. **Social media links** open in new tabs to correct pages: __PASS__ 

iv. **Visibility of contact information**all visible: __PASS__ 


## Notes on problems found during testing and problems during development
* Landing page i. the chevron did not align centrally with the header text. Corrected by changing the .row margin to 0. I also used position:absolute and percentage values rather than pixels to position it at different media breakpoints.
* Body i. white margin on the right hand side of the website on mobile devices corrected by changing .row to 0 margin
* Navigation bar iv. During development, the bootstrap 'scrollspy' would not appear on the navigation bar. I changed this by giving a nav item the 'active' class. I then had problems with the scrollspy not appearing on the navbar, although it was being activated. This was solved by changing the nabvar from navbar light to navbar dark and then targetting '.navbar-dark .navbar-nav .nav-link.active' in my css code to the desired background-color. The last probelm I had with the navigation bar was that whilst it worked to take the user to the correct section, the wrong item on the navlist was being highlighted. This was solved by changing the data-spy data-offset value from 0 to 170 in the html code.
* About vi. During testing, I realised that the About section when viewed on Safari had a very big top margin. I fixed this by removing an unnecessary 'wrapper' div from the alex image, switching the header to a seperate row, and targetting the columns themselves for padding and margins rather than the image itself. This solved the problem.
* Testimonials v. The read more button wasn't functioning at screen sizes over 1700 dpi. This was solved by giving the button position:absolute and a z-index of 10.
* I have noted this is my main README, but I also made a decision with my code to leave the media queries inline in the css for ease of changing specific details on the webpage at different breakpoints.


## Testing user stories

* **'I want to know about this person’s experience and what other projects they have worked on.’**
The about, projects and testimonials section will establish this. About includes information on their professional and academic background. Links to IMDb, which are visible across the site, give a professional feel and establishes their presence in the industry.

* **‘I want to get an impression of whether they are friendly and professional and see if they are someone I want to work with.’**
The copy is friendly, as are the call to action buttons to get in touch. The about section also gives a personal feel.

* **‘I want to be able to contact them easily.’**
There are multiple links to the contact section of the website: the landing page ‘contact’ button, ‘Let’s work together’ in the about section, from the navigation bar which is visible across the site, except the landing page. In the contact section, there is a contact form, email address, telephone and postal address plus links to LinkedIn Facebook, Instagram, Twitter and IMDb.

* **‘I want the website to be easy to navigate and the information to be relevant.’**
The website is very easy to navigate, as it scrolls from top to bottom. There is a navigation bar which shows clearly which section the user is viewing in relation to all other sections of the website. The copy and therefore information is short and to the point. Only essential information is present, including a summary of the individual, a summary of the services they provide and an overview of work they have undertaken. If the user wants more information, all this information is explorable via IMDb and social media, both of which are clearly visible at all times via ‘contact’ and the IMDb link on the navigation bar and landing page.
