Firstly; this project (as is), and upon not finding an /archive file, loads the tableView Cells 
very nicely, though I was forced to hand-code my own People.plist file -- the thing has a total 
of 30 Dictionaries, 30 persons I find interesting and/or to have been valuable to society. 

I have finished the guessing game feature, in which, once on the detail page, the textField 
fields are empty, save for place-holder prompts, and there is a label near the bottom which 
prompts the user to try to guess this man's name, Once both the first and last names have been 
entered with correct capitalization (and no trailing space) the label near the bottom turns 
to green and says "You got it!"
    
It is now time to try to debug the unarchiving (or archiving) of the images bug -- images taken 
from the photo lib do persist, but the original Cell images only show when loaded from the plist
 file. Subsequent runs result in good text and PhotoLib restorations, but the other Cell images 
are either not populated, or, are overwritten with nothingness.  

I should also like to fix the bug in which the Detail view image reverts to my hard-coded 
storyboard image whenever the persons last name is changed to an incorrect name. That I presume 
will require some fancy delegation of some sort, or, persisting a value in DetailViewController 
which could then be subsequently read by ViewController.swift and used to put-up the lost image.  

Since the text and added images are being loading from the /archive file, I do not understand 
why my images are not appearing as they should. As I understand it, that text and those Photo- 
lib images can only come from the same Person/people object in which the images are also being 
stored. Assuming I have stored them rightly. Please advise. Many thanks in advance. 
