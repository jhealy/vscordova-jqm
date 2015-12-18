# vscordova-jqm
Visual Studio Cordova and JQuery Mobile Step By Step

Rev 2015.1218.  Digging around there were no good tutorials covering how to add from scratch jquery mobile to a Visual Studio Cordova ( taco / phonegap ) project.  The source code files here are the output of my efforts.  Blog post coming soon.  Raw notes below.

Original source - http://learn.jquery.com/jquery-mobile/getting-started/

GOALS
* First, make it work like they have it
* Then, mod it to use local libs
* Then, mod it into cordova and make cordova have a base template

STEP ONE, AS IS
Create directory for project
Create "new website, empty asp.net".  Allows you to easily use the vs ide.
Key hassle was getting paths right.  Click on them in ide.  
    <link rel="stylesheet" href="https://code.jquery.com/mobile/1.4.5/jquery.mobile-1.4.5.min.css">
    <script src="http://code.jquery.com/jquery-2.1.4.min.js"></script>
    <script src="https://code.jquery.com/mobile/1.4.5/jquery.mobile-1.4.5.min.js"></script>

STEP TWO, LOCAL JQUERY
* Pull down / clone git repo
* Create scripts directory if one doesn't exist
* Create css directory if one doesn't exist
* Copy scripts ref'd above from git repo external to scripts

STEP THREE, CHANGE TO CORDOVA
* Create blank cordova
* Merge css and scripts folder from step two
* Manually merge in index.html, css in head, script refs in BODY, before cordova
* Manually merge in scripts and css ref

Feedback welcome....
