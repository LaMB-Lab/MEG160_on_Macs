# Running MEG160 on MAC OS X.

## Option 1: Use [Parallels][parallels].

### Pros:

* It certainly works. All you need to do is copy the MEG160 folder to your C:\ drive, and double-click "offlineMEG160.exe", in the MEG160/Bin folder.

### Cons:

* It costs money. A single [Parallels][Parallels] license will cost you around 80 dollars, although they offer discounted prices for bundles of two licenses.
* It requires a Windows installation CD. If you don't have one, you might have to buy one.
* It loads a full copy of Windows in order to run, and this might eat a lot of resources.

[parallels]: http://www.parallels.com/


## Option 2: Use [Wine][wine].

### Pros:

* It works well, especially if you use [Wineskin][wineskin].
* It's free!
* You don't need a Windows installation disk.
* It does not need to load a full copy of Windows, which probably makes it run faster.

### Cons:

* None that I could find so far.

### How to easily install [Wine][wine] for running MEG160:

1. Go to [Wineskin][wineskin], and download the latest version of the "Wineskin Winery.app", unzip the downloaded file and move it to your Applications folder.
2. Run [Wineskin][wineskin]. The "Installed Engines" window will list the versions of [Wine][wine] you might have installed. If you have none, you can do a clean install by clicking on the "+" button at the bottom of the window.
3. Select the latest [Wine][wine] engine version and click install.
4. Look at the "Wrapper Version" window. If it is empty, click on "Update".
5. Once you have the latest [Wine][wine] engine installed, you can click on the "Create New Blank Wrapper".
6. Name the new wrapper "MEG160.app".
7. Go to your LOCAL Applications folder (i.e., your_username/Applications), find the "Wineskin" folder, and see that "MEG160.app" has been created within.
8. Control-click on "MEG160.app", and select "Show Package Contents". You should see a window with three items: two folders ("Contents" and "drive_c"), and "Wineskin.app".
9. Copy the folder containing MEG160 to the "drive_c" folder (see figure).
10. Click on the "Wineskin.app", back on the MEG160.app folder. This will open the configuration dialog box (See figure).
11. Click on "Advanced".
12. On the "Windows EXE" menu, browse to the MEG160/Bin folder in "drive_c" to find "offlineMEG160.exe", and select it.
13. Click on Test Run. This should open MEG160.
14. If the test run worked, you can close the window and go back to your LOCAL Applications folder, find the "Wineskin" folder, and double-click on the "MEG160.app" within it. This should open MEG160.
15. Finally, copy the "MEG160.app" to your Applications folder. Now you have a MEG160 working like a regular Mac app.







[wine]: http://wiki.winehq.org/MacOSX
[wineskin]: http://wineskin.urgesoftware.com/tiki-index.php
