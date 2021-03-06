# Proposal-Work-Plan-Tool
This script is attached to a Google Sheet and allows one to generate Latex tables that may be included in a Latex document written for a research grant proposal using the "\input" command.  The tables describe the proposal's work-plan and associated schedules and labor distribution among the proposing team, and are rendered in 2 different versions:  an anonymous and non-anonymous version for inclusion in dual-anonymous-reviewed grant programs.  The tool allows one to make tweaks, additions, deletions and quickly re-render the new versions of these tables without worrying about human error or inconsistencies that arise when such edits are performed manually.

The below is a link to the Proposal Work Plan Tool spreadsheet on Google Drive:
https://docs.google.com/spreadsheets/d/13dq1RMxWeXLmCV8ZJ6xEEwG4FyxbGumCqLsV37Yvlyw/copy

and here is a link to the bio-sketch template that is also used in the script: 
https://docs.google.com/spreadsheets/d/1uX-W0NZhW2t6z13QanwLjNvYaXTFPxUg2D2XcdD8_gA/copy

If you hit the "Copy" button that appears when you follow the above links, copies of the spreadsheets will appear on the "Shared With Me" folder in your Google Drive. Those copies, which will include the attached script that makes Proposal Work Plan Tool work, are yours to use as you write your own grant proposals. You should move the Proposal Work Plan spreadsheet down into a designated folder for the proposal you are working on, which is where the latex files that are generated by the script will also be placed. 

The bio-sketch template should be moved into a folder that will hold the bio sketches of all the colaborators you work with on proposals.  This folder will serve as a sort of one-stop-shop for your collaborators to edit their bio sketches to keep them current over time, so that they don't have to create a whole new bio sketch every time you write a new proposal. 

To be explicit, let's say you created a Google Drive folder called "proposal2022" under another folder that holds all your proposal materials.  The folder/file structure that you start out with should look something like: 

          /AllProposals/ProposalsIn2022/ADAP2022/Proposal Work Plan verxxxxxxx

And then you might want to keep all the biosketches just under AllProposals, so you make a subfolder called bioSketches and then place the google sheet template under that folder:

          /AllProposals/bioSketches/biosketch

Copes of the biosketch google sheet template should be made, one for each collaborator you anticipate working with on the proposal. Something like:

          /AllProposals/bioSketches/BobSmith-biosketch
          /AllProposals/bioSketches/SallyJackson-biosketch
          /AllProposals/bioSketches/JanePerry-biosketch
          
The biosketch folder is one that can be added to over time, and each biosketch can be edited and maintained over time to keep the information up-to-date. 

The script should be ready to start accepting input, right out of the box. You may have to "accept permissions" when you try running "LIBRARY FUNCTIONS -> UPDATE LIBRARY" the first time.

Feel free to contact me if you run into permission problems or if you notice any bugs as you use the code.

*****NOTE: the below method works but is outdated -- a much easier process is now in place that works with GitHub -- I will make a new video soon, that shows how to use a one-button push to inject ALL the files generated by Proposal Work Plan Tool into your Overleaf project!*****
A video that describes Proposal Work Plan Tool and walks through all of its functions, including how to link the generated Latex table files on Google Drive with your Overleaf project, is provided at this YouTube link: https://youtu.be/a3tGQopb0QI

     %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
     %%%%%%%%%%  Thank you for your interest in Proposal Work Plan Tool !  %%%%%%%%%
     %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

Updates: ver 05192022 is the latest version
05/19/2022
  - Following using the scripts to get a proposal submitted this week, I've made more tweaks and one substantial change:  All files generated by Proposal Work Plan Tool now are also copied into a GitHub repository, where they can then be linked to your Overleaf project using a single button-push.  I will post instructions and video as soon as possible that demonstrate this wonderfully convenient new capability! 
  
05/09/2022
  - I've made several small tweaks to the code and have forgotten what most of the tweaks were.  But the MAJOR change was incoporating bio sketches.  Now, each collaborator can fill out the biosketch template (a google sheet) and maintain it over time.  The script sweeps up all the bio sketch information and then formats each bio sketch into a uniform template. The advantage of this approach is that one can list ALL of their publications, etc. but use the righthand columns in the sheet to indicate whether that publication should be listed in the bio sketch for that proposal or not.  Some publications might be relevant only to certain proposals, but the spreadsheet allows one to store all that information in one place. 
  
12/10/2021
  - corrected an error in the script that kept some of the tables from rendering correctly because of an indexing issue that caused the code to grab the wrong columns of FTE data. 
  - corrected the script so that it now properly removes any columns of years in the FTE tables for which the proposal has no FTEs assigned.  For example, if the proposal is only a 2-year grant, then only 2 years will be shown in the LAtex tables and will not waste space showing years 3, 4 and 5 that have only 0 FTEs in them.
  - corrected a few minor bugs (like the FTE sub-totals in the upper right cover of the TASKS tab not showing correct in-kind contributions).
  - added ability to select "student" collaborator designations ("st(1)", "st(2)", etc.)
  - changed the cell in the  ANONtasks tab (a hidden tab) that controls the table footnote to be a more generic text, and flagged the cell so that it can be easily found by the user and the text changed to whatever is desired (a note is now appended to that cell to describe how to change the text). 
  - flagged the cells in several other latex template files (e.g., NOTANONtasks, NOTANONpersonnel_work_effort, etc tabs) to indicate where one might change the color schemes of the Latex tables, if desired -- see the notes that are attached to the flagged cells for details). 
