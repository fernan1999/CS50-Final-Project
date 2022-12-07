# CS50-Final-Project
Fernando Soca | Harvard College 2022
https://fernan1999.github.io/CS50-Final-Project/

# Simple User Guide
  My project is a voter guide for Palm Beach County, primarily based on the Palm Beach County Democratic Party's recommendations for the 2022 midterms. Since I recently moved to Palm Beach County, I looked for similar recommendations as I prepared to cast my vote and found they all had one of two issues. Either they didn't state the candidate's platform and only told you who to vote for, or if they did include it they missed many local candidates as they were more focused on major races. I wanted to get to know the candidates who would represent me rather than just follow a down-ballot guide and I also wanted to understand why I shouldn't vote for others and where we disagreed. 
  
  This is primarily designed for web browsers and not meant for mobile. It was easier to perfect the layout of the page in one single form than try to account for different options, based on my skill levels. 

  The Home Page features a map of Palm Beach County by zipcode that allows you to right-click to open it in a new tab to zoom into the picture and determine your area. The zipcode must be used in the official Florida website, found here (https://www.flsenate.gov/senators/find) and here (https://www.myfloridahouse.gov/findyourrepresentative) to determine your representatives. The navigation bar takes you to the different pages to see the recommendations and the "Sample Ballot" option allows you to open a new page with the official 2022 sample ballot that allows you to print or download it.

  To make it easy to use, every option on the ballot is divided into one of 5 categories: National Candidates, State candidates, Local Candidates, Justices, and Referendums. Within each category, if it's a candidate, is their name and picture, statements made on their official website or to a local newspaper, and a recommendation as to who to vote for and the reasoning. 
  
  National Candidates include indepedents as their participation in nationwide races is far greater than statewide, of which few even run, and thus deserve representation in the guide. 
  
  If it's a judge looking to be retained, only Supreme Court Justices with a "NO" recommendation are mentioned as guided by the Palm Beach County Democratic Party with a short reasoning. For Circuit Judges recommendations, within the Justices page, you can find the official Florida Bar Association recommendations determined through an annonymous poll of its members, as a seperate document to print or download and follow along. We based our recommendationa on circuit judges on this poll as a link to it rather than other opinions partly due to the lack of knowledge on recommendable quallities and also the Palm Beach County Democratic Party does not take a position in these races either.
  
  In referendums, you can find all the state and county questions on the ballot with their specifications as well as a simple recommendation, once again based on the PBC Democratic Party. This is because the referendums are generally straightforward in their explanation and often times there are very clear choices as in 2022.
  
  The official PBCDP Voter Guide this is based on can be found here: https://qrcodes.pro/nRZfvn
  
 # Technical Details

  I picked a Red, White and Blue, color scheme to give it a patriotic vibe. The Blues are the official hex codes for the Democratic Party's baby blue and darker blue shades. The #00AEF3 color code is used for the background while the #0015BC is used for the navigation link colors. The Red #FF0000 to determine the active link, and the White #FFFFFF for any large font text and the shading around the active link. The recommendations are in red to find it quickly, the sizes of the staements and reasonings fonts are different so that the candidate statements stand out. Every candidate has a similar ratio in picture size to their opponent's as to avoid any bias in presentation. As well as statement lengths were made of similar size to the best of my attempts, sometimes candidates offered far less than their opponents both on their website and to public sources, to once again avoid any bias in presentation. The reasoning, as its clearly and intentionally biased, is slightly smaller in size font and varies in length, because its not as important as what the candidates themselves represent. 
  
  The Background is the same for every page, I like the simple pleasing aesthetic, with a general theme of title, navigation bar, and bookending logos based on their relation to the page's subject, followed by races and recommendations. It thus is quite clear in the html files, the general pattern the pages follow of creating rows and columns to correctly position the individual images and texts within the page. I used direct links to the images to avoid having to directly host them and make the code easier to tranfer as the image links should work for the foreseable future. And for similar reasons, linked to the direct files for the sample ballot and circuit judges in the navigation bar. 
  
  The bookending logos differ based on their subject matter, whether being the seal of the Senate, the seal of the State Senate, or seal of Palm Beach County, as to add some interesting easter eggs for those that notice and enforce the theme. The pictures of the candidates were pulled from a variety of sites due to resolution restrictions and were chosen for similarity in pose, outfit, and setting to avoid bias. The pictures of justices were pulled from their official Florida Supreme Court portraits.

  To find the Home Page html file, its in the main CS50 Final Folder as index.html with its accompanying CSS file, for formatting, in the same folder as styles.css. The index file contains refences to the Bootsrap style sheet as well as the previously mentioned style.css style sheet to properly format the document. Bootstrap, and its stylesheet, are used for the navigation panel in general and more specifically for the "active" icon shading. The Bootstrap required plugins are thus also included to run the navigation bar properly. 
  
  In each clearly labeled subfolder within the CS50 Final folder, you will find the individual pages' html, labeled with their initials according to folder name, and their accompanying css file simply labeled style.css. With each individual html file requiring the same Boostrap stylesheet and plugins as the homepage with only the Justices page's navigation bar differing and having one more option than all the others. This was for the circuit judge recommendations that are only relevant in the justices section. 
  
  The site is being hosted on Github as part of the free project pages option. You can upload the files in your own repository, ideally using the same name as to avoid address edits, and host the entire website through pages for free. You would just have to go to repository settings and deploying it from the corresponding branch it's located in. This is a great way to actively edit and preview your build, as well as having the ability to share it for viewing and the ability to open it to collaborators before official publishing.
  
  # Future Improvements
  
  I consider the website a success in both its establishment of a framework to work on in the future and its decent coverage of underepresented races. Truth is, there are far too many races to adequately cover and discuss in the scope of this project. While I hated not covering national candidates more, especially for the House, I considered it a worthy trade off to focus more on local elections that aren't mentioned in guides or newspapers. In the future, the addition of all races and their subdivision by zipccodes, would be the primary goal. The main issue with the deployment of a zipcode organizer is that districts have already been redrawn from the last election and will surely be redrawn again, placing a hurdle in an automated system. This is why users are referred in the beginning to the 2 Florida websites, needed during every election, to find out their districts. As neither even offers the complete information to the voter as to who the incumbent is. 
    
   While the general aesthetics of the site doesn't adhere to modern sleek and intuitive design principles, it fondly reminds me of the simple but useful wbesites of prior years that are more content than show. I personally care about the color schemes most of all as I find it hard to read text sometimes depending on which are used in conjunction since I'm Red-Green colorblind. I also get flustered with overcomplicated drop downs and interactive options when I simply want a quick and easy reference for information so I tried to keep it simple and functional, as well as aesthetically pleasing. 
   
   Big addition to the site that is possible but would expand the scope of this project would also have been an addition of an elections results page that would import the CSV file from the official PBC database to update automatically. 
