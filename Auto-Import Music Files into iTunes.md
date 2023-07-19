<p align="center">
<img src="https://macstores.vn/tin-tuc/wp-content/uploads/2021/12/20211212_61b624ba2ca1e.jpg" />
</p>

<h1>Creating a Desktop Link to Auto-Import Music Into iTunes</h1>
This walkthrough details how to create a batch file to automate the import of audio files into iTunes library.<br />


<h2>Environments and Technologies Used</h2>

- Windows 10
- iTunes
- Batch Files

<h2>Operating Systems Used </h2>

- Windows 10

<h2>Overview</h2>

- Step 1
  - Install iTunes (If not done so already)
- Step 2
  - Create a folder on Desktop to copy music to be imported
- Step 3
  - Create batch file with move command
- Step 4
  - Copy music files into folder on Desktop
- Step 5
  - Click on batch file to import
  
<h2>Detailed Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Step 1: Install iTunes if you have not done so already. This can be done either through the Windows store or by navigating directly to the iTunes website.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Step 2: Create a folder on the desktop and call it "Music to be Imported"
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Step 3: Create a batch file with a command to move files from the folder on the desktop to the auto import folder in the iTunes directory. To do so, open a notepad file. Type in the following below:
  
  @echo off <br>
  move [source folder] [destination folder] <br>
  
  Fill in the brackets with the file path for the source folder that you created in step 2, and the destination file path for the auto-import folder in the iTunes directory. Usually it is located in C:\Users\[username]\Music\iTunes\iTunes Media\Automatically Add to iTunes. When typing in the file path for the source folder, make sure to add \*.* at the end, which tells the command to execute for every file in the folder. <br>

Example:
  @echo off <br>
  move C:\Users\[username]\Desktop\"Music to be Imported"\*.* C:\Users\[username]\Music\iTunes\"iTunes 
  Media"\"Automatically Add to iTunes" <br><br>

  Save the notepad file onto the desktop and save it as a .bat file by typing .bat at the end of your filename.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Step 4: Copy music files into the import folder that you created on your desktop. NOTE: These files will be imported into iTunes and will be removed from this folder when command is executed. Best practice is to copy the files into this folder, instead of moving.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Step 5: Click on bat file on the desktop and then open iTunes to find your new songs imported into your library.
</p>
<br />
