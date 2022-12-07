# Implementation

This is primarily designed for web browsers and not meant for mobile. It was easier to perfect the layout of the page in one single form than try to account for different options, based on my skill levels. 

For all the pages, I used the bootstrap stylesheet, plugins, and script, to run the nav bar. The nav bar has straightforward file links through github to each individual page's html and a name for each link labeled "national candidates" and so on. File links were used as an easier way to reference different pages within github and host them. The nav bar requires that the current page always be labeled as 'active' to correctly format its shading, and a CSS addition (labeled) was required to overide the Bootstrap style sheet for the color of the 'active' shading on the tab, as well as additions to overide the format of the text size, color, and padding of the nav bar tabs.

The only 2 tabs that open in a seperate page are 'Sample Ballot' and 'Circuit Recommendations' as to not have the user leave the webpage and have to return via browser buttons. This way the user can open the documents to view, download, or print, and stay on the page and still navigate using the nav bar. This is done through a simple 'target:blank' addition to the code. 

I also used individual style.css documents corresponding to each HTML since to code faster, I just created a general theme to copy and paste with fill in the blank areas and didn't want to have to edit each individual identifier in both the html and css to make them unique. While it saved me time, it requires seperate css files as to not merge the different formattings across the pages accidentally. 

The CSS files all share the same name as they're in individual folders and the file link remains the same as long as this continues. If they were all in one CSS folder, the names would have to differ. 

For each individual element, whether text, image, or titles, I placed them within a row or cell as to better format their positioning, attributes, and make them better organized within the html file. Through this, each text, image, and title, is centered off each other without having to precisely float them invdividually. Each row and cell has unique CSS values since I had to format them individually also according to their content size to better display them by adjusting the padding and dimensions for example. Few rows share similar enough attributes to combine them in CSS files. Individual textboxes shared many similar attributes when it came to font size, color, and weight, but in things like padding differ greatly based on their individual requirements to display. Once coded, I used visualizers like W3 schools, Github pages, and Grapejs to fine tune the CSS visually and get the formatting exact for PC screens. I attempted the mobile conversion but was unsuccessful.

Every title or name is in white for priority. Every text box is in black for readability. And every recommendation is red for the ease of finding them. the mao in the homepage has auto margins on the left and right to center correctly. 

The pages are desgined so that in the future I can simply edit them by copying and pasting the new candidates info for the next election to update the website without having to reformat it.

I used the Github Pages  to host the website for free through a dedicated url found at https://fernan1999.github.io/CS50-Final-Project/ 

# Technical Details
I picked a Red, White and Blue, color scheme to give it a patriotic vibe. The Blues are the official hex codes for the Democratic Party's baby blue and darker blue shades. The #00AEF3 color code is used for the background while the #0015BC is used for the navigation link colors. The Red #FF0000 to determine the active link, and the White #FFFFFF for any large font text and the shading around the active link. The recommendations are in red to find it quickly, the sizes of the staements and reasonings fonts are different so that the candidate statements stand out. Every candidate has a similar ratio in picture size to their opponent's as to avoid any bias in presentation. As well as statement lengths were made of similar size to the best of my attempts, sometimes candidates offered far less than their opponents both on their website and to public sources, to once again avoid any bias in presentation. The reasoning, as its clearly and intentionally biased, is slightly smaller in size font and varies in length, because its not as important as what the candidates themselves represent.

The Background is the same for every page, I like the simple pleasing aesthetic, with a general theme of title, navigation bar, and bookending logos based on their relation to the page's subject, followed by races and recommendations. It thus is quite clear in the html files, the general pattern the pages follow of creating rows and columns to correctly position the individual images and texts within the page. I used direct links to the images to avoid having to directly host them and make the code easier to tranfer as the image links should work for the foreseable future. And for similar reasons, linked to the direct files for the sample ballot and circuit judges in the navigation bar.

The bookending logos differ based on their subject matter, whether being the seal of the Senate, the seal of the State Senate, or seal of Palm Beach County, as to add some interesting easter eggs for those that notice and enforce the theme. The pictures of the candidates were pulled from a variety of sites due to resolution restrictions and were chosen for similarity in pose, outfit, and setting to avoid bias. The pictures of justices were pulled from their official Florida Supreme Court portraits.

To find the Home Page html file, its in the main CS50 Final Folder as index.html with its accompanying CSS file, for formatting, in the same folder as styles.css. The index file contains refences to the Bootsrap style sheet as well as the previously mentioned style.css style sheet to properly format the document. Bootstrap, and its stylesheet, are used for the navigation panel in general and more specifically for the "active" icon shading. The Bootstrap required plugins are thus also included to run the navigation bar properly.

In each clearly labeled subfolder within the CS50 Final folder, you will find the individual pages' html, labeled with their initials according to folder name, and their accompanying css file simply labeled style.css. With each individual html file requiring the same Boostrap stylesheet and plugins as the homepage with only the Justices page's navigation bar differing and having one more option than all the others. This was for the circuit judge recommendations that are only relevant in the justices section.

The site is being hosted on Github as part of the free project pages option. You can upload the files in your own repository, ideally using the same name as to avoid address edits, and host the entire website through pages for free. You would just have to go to repository settings and deploying it from the corresponding branch it's located in. This is a great way to actively edit and preview your build, as well as having the ability to share it for viewing and the ability to open it to collaborators before official publishing.

# Improvements for the Future

To combine CSS stylesheets into one single document by identifying and renaming each element corresponding to a new CSS. And to host the images and files locally rather than depend on external servers. 

Ideally, in the future when all candidates are listed, I can just comment out the races that aren't happening that election cycle and still maintain the same framework for every election with applicable fill in the blanks. 

Use float attributes to eliminate the need for rows and columns to organize elements spatially. 
