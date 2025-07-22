```
What follows is from an email to Charlie Duke, July 22, 2025...
```

Yes, I have copied all the images to a new home in the cloud.  Those URLs will be of the form: 
 
https://gcsmbstorage.blob.core.windows.net/objs/physics_museum/ac_004_turkish_tubaphone.jpg
https://gcsmbstorage.blob.core.windows.net/smalls/physics_museum/ac_004_turkish_tubaphone_sm.jpg
https://gcsmbstorage.blob.core.windows.net/thumbs/physics_museum/ac_004_turkish_tubaphone_tb.jpg
 
I also have a new repo for you to fork and work from: 
https://github.com/Digital-Grinnell/GCCB-physics-museum
 
Changes to that repo automatically update https://yellow-tree-09e303e1e.1.azurestaticapps.net/.
 
That is a public repository built from our GC template and merged with your data.   Note that it currently uses the `pmeta4-24.csv` file for metadata, but that sheet currently points to the images that Libby prepared, NOT your latest images.
 
I left Libby’s old image URLs intact because I find them much easier to work with.  We have a convention of using short names for the image files in cloud storage, like `ac_001.jpg`, `ac_004.TIF`, etc.  That way I don’t have to know the details of the full image name to populate the CSV file.    
 
Unfortunately, Libby’s files don’t entirely follow our convention because she used a mix of extensions, like `.jpg` for some files, but `.JPG` for others.  I like to have all those extensions in lowercase too, but that’s an easy inconsistency to deal with.   The long file names are much more difficult to accommodate, but still doable. 


## Suggested Workflow 
 
- Fork https://github.com/Digital-Grinnell/GCCB-physics-museum to create something you can work with,  
- Clone your fork to your workstation, probably `git clone https://github.com/dukecld/GCCB-physics-museum`,  
- Make a new branch `git checkout -b <branch-name>`,  
- Produce a new CSV file from your script giving it the same column headings and structure as you find in `pmeta4-24.csv`, then. 
- Edit your new CSV filename into `_config.yml` (line 37), and. 
- Build the site locally.  Repeat this step as needed until you have things working as you like.  
 
- Once you are satisfied with your changes, `git add .`, `git commit -m <message>` and then `git push` them back to  `https://github.com/dukecld/GCCB-physics-museum`.  
 
- Navigate to https://github.com/dukecld/GCCB-physics-museum in a browser and open a pull request that I can review and approve to update https://github.com/Digital-Grinnell/GCCB-physics-museum.  
 
- Whenever the main branch of https://github.com/Digital-Grinnell/GCCB-physics-museum is updated it automatically generates a new site at https://yellow-tree-09e303e1e.1.azurestaticapps.net/.  
 
I know it looks like a lot of work, but I think if you try it once you’ll find it works pretty well, and steps 1-5 only happen one time, they do not have to be repeated. 
 
Let me know if any of this need’s clarification, or if you just want to hand off much of this (we really need you most for Step 4) to me and Sol, just say the word. 