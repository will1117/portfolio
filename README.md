<!-- The process behind building my website -->
From my wireframe concepts, I wanted my portfolio to breakdown into different sections that categorized the images by genre, so that potential clients can see examples of my works broken down into specific mediums. I decided to create three seperate galleries in columns/row formats, with each gallery preview displaying the most eye-catching images from each genre, with a dropdown button expanding the galleries for further exploration. 

I started with the header. I wanted my main menu to turn into a hamburger menu an minimum/medium width, and expand at a large size, so I turned it into a collapse menu, with "navbar-expand-lg" when it hits a large size. Next I added the logo, and social media links by adding Fontawesome Icons and adding links to the text. 

For each gallery, I created rows with a number of columns per row depending on the image size/visibility. (All galleries for the mobile version have 2 columns per row). I chose to have two rows for the gallery preview, as I felt it was a reasonable amount of content for a preview. I then created collapse buttons that would expand the galleries to show 2-3 more rows of images. 

I then added my footer at the bottom using the same colour pallette as my previous website, with copyright and social media icons included.

Finalization included adding librairies, google fonts, the banner image, and skip links. 


<!-- Challenges faced -->
1. Skip link underlines - As I was styling my skip links, I wanted the underline to match the colour of the text, but not stand too strongly. Using bootstrap's guide, I was able to use "link-underline-light" to style it white, and "link-underline-opacity-50" to set the line opacity to 50%.

2. Styling the menu - When I was styling the nav bar at the large size, I was having lots of difficulty with centering my items and buttons breaking outside of the container. To fix the centering issue, I applied "mx-auto" to my menu button, dropdown items and navbar-nav container. I also changed the width of my menu items so that their large size would not expand out of bounds.

3. Header background image - I wanted my background for the header to match that of my first website, which had a black and white picture of a leaf set as the background cover. I used "bg-secondary" to define the background area that I wanted the image to go in, and used "background-image: url(images/header-img-2.png);" tp add the image itself.

4. Gallery expand button - Because there were no guides on how to make grids expand in a similar fashion to the hamburger nav menus, I experimented with the "collapse" feature used in the nav menu. I divided the gallery preview images' rows and the expanded gallery images' rows into two seperate divs, giving the expanded gallery's div its own ID ([Name]Gal, short for [GenreName]Gallery) and a "collapse" property. I then added a button underneath the gallery div and gave it properties of data-bs-toggle="collapse" and data-bs-target="#[Name]Gal" so that when the button is clicked, it triggerd the collapse of the items within the gallery div.

5. Adding animations to images using library - I chose to use the "Animate on Scroll" library by michalsnik on github to animate my images when scrolling down. I added the following properties used in their github examples:
    data-aos="zoom-in" - Creates a zoom in animation 
    data-aos-anchor-placement="center-bottom" - plays the animation when center-bottom of image is reached
    data-aos-duration="700" - animation duration
I had difficulties with having the animations play properly, so instead of adding the animation properties to the container, I added them to every individual image.


<!-- Sources -->
Bootstrap: https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css
Fontawesome Icons: https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css
Scroll Library: https://michalsnik.github.io/aos/
Google font: https://fonts.google.com/specimen/League+Spartan

All images used in my website are my own.