# Implementation

This is primarily designed for web browsers and not meant for mobile. It was easier to perfect the layout of the page in one single form than try to account for different options, based on my skill levels. 

For all the pages, I used the bootstrap stylesheet, plugins, and script, to run the nav bar. The nav bar has straightforward file links through github to each individual page's html and a name for each link labeled "national candidates" and so on. File links were used as an easier way to reference different pages within github and host them. The nav bar requires that the current page always be labeled as 'active' to correctly format its shading, and a CSS addition (labeled) was required to overide the Bootstrap style sheet for the color of the 'active' shading on the tab, as well as additions to overide the format of the text size, color, and padding of the nav bar tabs.

The only 2 tabs that open in a seperate page are 'Sample Ballot' and 'Circuit Recommendations' as to not have the user leave the webpage and have to return via browser buttons. This way the user can open the documents to view, download, or print, and stay on the page and still navigate using the nav bar. This is done through a simple 'target:blank' addition. 

I also used individual style.css documents corresponding to each HTML since to code faster, I just created a general theme to copy and paste with fill in the blank areas and didn't want to have to edit each individual identifier in both the html and css to make them unique. While it saved me time, it requires seperate css files as to not merge the different formattings across the pages accidentally. 

The CSS files all share the same name as they're in individual folders and the file link remains the same as long as this continues. If they were all in one CSS folder, the names would have to differ. 

For each individual element, whether text, image, or titles, I placed them within a row or cell as to better format their positioning, attributes, and make them better organized within the html file. Through this, each text, image, and title, is centered off each other without having to precisely float them invdividually. Each row and cell has unique CSS values since I had to format them individually also according to their content size to better display them by adjusting the padding and dimensions for example. Few rows share similar enough attributes to combine them in CSS files. Individual textboxes shared many similar attributes when it came to font size, color, and weight, but in things like padding differ greatly based on their individual requirements to display. Once coded, I used visualizers like W3 schools, Github pages, and Grapejs to fine tune the CSS visually and get the formatting exact for PC screens. I attempted the mobile conversion but was unsuccessful.

The pages are desgined so that in the future I can simply edit them by copying and pasting the new candidates info for the next election to update the website without having to reformat it.

I used the Github Pages  to host the website for free through a dedicated url found at https://fernan1999.github.io/CS50-Final-Project/ 

# Improvements for the Future

To combine CSS stylesheets into one single document by identifying and renaming each element corresponding to a new CSS. And to host the images and files locally rather than depend on external servers. 

Ideally, in the future when all candidates are listed, I can just comment out the races that aren't happening that election cycle and still maintain the same framework for every election with applicable fill in the blanks. 
