# Basic Portfolio assignment

### Links
Basic portfolio on [Github Pages](https://www.google.com)

Easier homework: [Github Pages](https://jeffreylowy.github.io/HW-Wireframe) | [Repository](https://github.com/jeffreylowy/HW-Wireframe)

### Template

#### HTML
After reviewing the images provided with the assignment, I sketched out a basic page, taking note of all of the design elements shared across all of the pages. Since the main content area is the only piece that changes across each page, I decided I should create a template. 

#### CSS
To save time, I copied all the CSS specific info from the assignment instructions into a commented section at the top of my style.css file. I mainly created the CSS while designing the HTML template from top to bottom (header > content > footer). My CSS file began with only a header, nav, content, sidebar and footer sections. Before I started coding, I knew I wanted to accomplish the sticky footer bonus task. I added page specific CSS between the content and footer. I grouped each page section and labeled them with a comment to make them easier to locate as I moved throughout the file.

### Pages

#### About / Index

Pretty straight forward. I floated the image to the left and added margin to push the text away from the picture. I gave the floated image a class so that the float wouldn't affect the images on other pages. Also, I did not want to wrap it in another div, span, etc.

#### Contact

To stack the elements, I made each a block. I then targeted the inputs by their type. Mainly because I didn't want to make the submit input a `<button>` element, and I did not want the button to inherit the width from the other inputs. I changed the text area's font-family to match the other content, rather than use the browser's default style.

#### Gallery
I wanted each column of images to hug the left or right side. Adding margin-right to the portfolio items would work for the items on the left, but would prevent the items on the right from touching the container's border. So, I wrapped the portfolio items in a class named 'portfolio'. This allowed me to easily target and add margin-right only to the odd numbered portfolio items (items on the left).

I could have set the images as the background for each item in stlye.css, but I did not want to create classes or ids specific to each portfolio item. In case there were ever hundreds of items, I wanted to keep the image, and it's title 100% in the HTML. I set the position of the portfolio items to relative and the images and their titles to absolute. The order of the HTML allowed me to bypass using z-index to layer the image and the title.


### Bonus

1. Targeted the `<a>` tags in the nav to make them teal & underlined when hovered.
2. Added a CSS filter property to the portfolio images. The grayscale value is adjusted on hover. 
3. Created the sticky footer based on one of the suggestions from the CSS tricks article provided in the instructions (though I had to tweak it a bit).