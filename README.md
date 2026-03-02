#GENERAL NAVIGATION:#  
The site consists of the main landing page which is made up of three main blocks: header/navbar, hero/bio, Worked with.  
  
The header/navbar and Work with section will appear on all pages other than the Recent Work pages (main Recent Work page and children)  
  
The Recent Work page will have all of the items from the "Worked with" section in row format, maybe with a brief description, the rows then linking to their own page which could have expanded detail of the work experience and a link to the company's website.  The icons in the "Worked with" section on the main page would link directly to the expanded page for each company  
  
There is a "Testimonials" page that's a simple row layout with formatted quote and attribution text to be filled in  
  
The "Get In Touch" link in the navbar stays on the main landing page, but makes the social media icons in the header swell, pushing the navbar out to fit along with them.  There is then a "click anywhere" script that returns the socials and header to normal state  
  
  
#COLOR PALETTE:#  
I wanted to practice coordinating the color palette across the site and using variables to easily update color classes(?) site-wide, so I found the extension "macOS Color Picker" for VS Code to use its eyedropper tool so I could sample the colors from the profile picture (had some fun making the background color a sample of Brad Pitt's skin tone, his blazer color is the hover color for the socials, the socials themselves are sampled from the sunset behind Brad, the header, text, and Worked with colors are sampled from Brad's hair and beard)  
  
#ANT MARCH:#  
The Worked with section in the Figma looked to be begging to have an ant march, so, since I'd never done one, I had chat help me with this, it took some tweaking, the params that it had by default didn't look good, but I'm pretty happy with how I got it looking in the end.  There are a couple problems with it that I couldn't fix, listed below   
  
  
#BUGS & FUTURE IMPLEMENTATION:#  
1. Ant march: there's a jump in the loop at the end of the first list of icons, when it restarts on the second list - it seems to be due to some padding on the first item in the loop, which is also making the space between the last item of the one list and the first of the next bigger than it's supposed to be  
  
  
2. I tried to paint the ant march with a gradient so that the icons would change color along the gradient as they scolded past - I was able to get the gradient applied to the box (as a background), or to the icons themselves (the whole gradient happening on each individual icon itself), but I wasn't able to get the effect I was trying for.  I'll want to come back figure this one out as I think it'll be a nice look, and useful in other applications  
  
3. There are media queries for desktop, tablet, and phone resolutions.  This is not very clean, I ended up adding a query for desktop to force something to work, but it seems like there shouldn't need to be that query as I built it desktop-first, I'll want to clean this up.  I think I'll try mobile-first design next time as that seems to be the climate we're in, so then I should have a query to switch to tablet, then one to switch to desktop (and not one for phone)  
  
4. The "Get In Touch" swell effect on the social icons makes them run off the edge of the navbar at screen widths near the break from desktop to tablet, and then again at ultra narrow res (narrower than iPhone SE)  
  
5. If staying with the social icon swell for "Get In Touch" should add an email icon, maybe a phone icon  
  
6. I was pretty happy with making the hamburger menu constrain to the 80% width to match the header and Worked with sections, which then made it make sense to round the corners as well, which gave it a nice modern look.  I tried to apply the sunset colors to the hamburber menu rows, but all I was able to do was apply them as background to the li text items.  This is something I'd like to figure out how to do - I suspect it will require handling each link as its own entity rather than as ul, which abandons the elegance of that approach, but maybe it would be worth the extra coding I'm anticipating to be able to get that functionality (or maybe it's easier than I'm thinking)  


