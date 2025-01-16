This post will be a little technical, a little bit complicated, but very important - we will be installing MySQL Workbench and a MySQL Server. You'll need both in almost every post of our SQL collection: SQL INSERT Statement, SQL UPDATE Statement, SQL DELETE Statement, SQL Best Practices;
Installing MySQL
Let's look at MySQL's official website.
Select the "Downloads" section and click on "Community", as we would like to show you how to download a file that is open-source and free.
We will go through the installation process for a machine operating on Windows, but please remember the video will be useful if you are installing MySQL on a machine running on Mac OS or Linux, as what needs to be done is similar.
So… I'll click on "MySQL on Windows".
You can either download MySQL components and tools separately or download the MySQL installer then choose which tools you would like to install from there. The second option is much quicker and easier to implement. That's why we will select the Installer.
Scroll down to where you see two versions of the installer. Before discussing them, please pay attention to this important note.
MySQL Workbench, its installer, and all software tools are constantly being updated to solve different bugs and whatnot. This is why, during the installation process, we can be left with the impression that the components we are installing are different versions. This is not an issue. Usually, the changes between different versions are marginal. That's why they would not affect the execution of the tasks presented throughout this post.
So please, if you are about to download a version of MySQL that is older or newer than the one you see in this post, remember apply all code used in our SQL posts and exercises without experiencing issues.
Now that we said that, let's focus our attention on the two options provided. The first one is suitable for those of you who have internet connection (throughout the installation process).
The second will be appropriate if you will just download the file and then install the software when you are offline. Naturally, the first one is better. Select the relevant "Download" button.
A page offering you to log in or sign up for an Oracle Web account will open. This is not an obligatory requirement, so you can press "No thanks, just start my download."
Then, a new window will pop up. Select the directory where you would like the installer file to be downloaded. When you've done that, click on "Save".
We don't need the MySQL page anymore. So, you can open the installer and wait for it to load.
As this is happening, depending on the version of your operating system and its settings, you might get a message asking you to allow certain apps to make changes to your device. Please, agree and continue.
Then, a prompt box will appear asking you for an update. You don't need it at the moment, so please press "No".
Right!
This is the MySQL Installer window. "To proceed you must accept the Oracle Software License Terms". You can do this by ticking this little box at the bottom of the window and then clicking on "Next".
What comes up are a few different Setup Types. We need not discuss all of them. For our purposes, "Custom" will allow us to specify the tools we need. So, let's select "Custom" and click on "Next".
Ok. At this stage, you can select the products to be installed. In the next section of this post (The Client-Server Model) you will find a PDF file explaining why we will need "MySQL Workbench" and a MySQL server.
First, expand the Applications section, then the "MySQL Workbench" subsection, and then click on the name of the tool and on the little green arrow to move it to the section of products or features to be installed.
Good.
Now, we must add a server. Expand the "MySQL Servers" section, then the "MySQL Server" subsection, and finally choose one of the two versions - the 64-bit or the 32-bit (which is called X 86). I will be coherent with the Workbench feature, so I'll select the 64-bit version.
Great!
We are done selecting features. Click on "Next" to move to the next stage of the installation process.
Press "Execute" to install Workbench and the MySQL Server package.
Once this is done, the status of both features will be marked as "complete". This means we are ready to proceed. Let's click "Next" again.
You'll move to the stage of product configuration - the last step of the installation process. The status of the Server should become "Ready to Configure". This means you can move a step further.
Ok!
Now, you will adjust the configurations of your server. We need not go into details. Keeping the default settings in the next two pages will let us install a version that will suit the purposes of our SQL posts. So, just click "Next" two times.
A-ha! This step is crucial, and it must not be overlooked! Here, you are being asked to set up a root password. And you mustn't forget your password, because it will be hard to change or recover it later. Otherwise, "root" refers to the main connection established between you, as a user and the MySQL server you are about to install.
Press "Next" once more, and…
Keep all the settings that just appeared as they are, especially the ones regarding the start of the MySQL server at System Startup. Unless you leave this option ticked, you must set up the server manually when you use SQL, and that's not a straightforward operation.
Ok, press "Next" again.
You will be offered to install a plug-in that contains improvements on previous versions of Workbench, but it will not be relevant for us right now. So, please skip this step by clicking "Next" once more.
And… finally… "Execute"!
Wait until the installation is complete and click on "Finish".
You won't need to go through the wizard that appears, so click on "Next".
Then, leave the tick on "Start MySQL Workbench after Setup" and press "Finish".
Now, Workbench will load and you can set up a connection between Workbench and the MySQL Server.
We'll learn to do that in the section "Setting up a connection".
The Client-Server Model
In this PDF file you will find a visualization that explains which MySQL features we must install and why.
The program we will be working within this post is called MySQL Workbench. It is the Oracle visual tool for database design, modelling, creation, manipulation, maintenance, and administration. Professionals refer to this type of software as "Integrated Development Environment" or IDE. So, Workbench will be our IDE.
And, if you wonder what Oracle is, this is the software company that owns the MySQL version of SQL.
You could also wonder why we would need a server. Sticking to the basic theory of operation of computer networks, MySQL Workbench acts as a client program - a client of a MySQL Server. The server is, practically, nothing more than a machine that provides data and services to the same or other computers. The data could be provided locally or online. Regardless whether the server is installed locally on your computer or is being accessed remotely over the internet from another computer, you will need a Server to use MySQL. In our case, we installed the server locally.
Briefly, the server will perform all calculations and operations you execute in Workbench. You will be writing queries through the Workbench interface, in the form of raw code, which MySQL server understands and processes. Finally, when it finalizes its calculations, it will bring the respective results back to you in the form of an output displayed on your screen.
Setting up a connection
All right!
MySQL Workbench is the official Graphical User Interface tool, or GUI tool, for MySQL. This means it will be the tool that will show us "communication" with the MySQL server.
Fantastic!
First, to access Workbench, we must set up a connection between your GUI and the MySQL server. Otherwise, the two will not be linked, and you cannot execute any code.
A connection has been created for you.
Click on the rectangle you see here then insert the password you designated during the installation process. Press "Ok" and… here you go.
Now you can use the MySQL Workbench!
Getting acquainted with the interface will be the focus of our next section. Before doing that, I would like to tell you that you can load more than one connection at a time in your GUI. All connections will be under different tabs, next to the house in the upper left part of the screen.
Should you press the house icon, logically, you'll immediately jump to the main tab, showing your MySQL connections. We can see just one. Ok.
If you want to go back to the connection already loaded, you must click on its name. And, to close it, just press this little close sign.
Nice!
If you need to set up a connection, you must press the little "plus" sign on the right side of the "MySQL Connections" label.
In the window that pops up, you will see several empty fields. The first one is compulsory, as the text inserted will be the name of the connection you are about to establish. Then, you can click on "Test Connection" to see if, after typing the password assigned in advance, the connection works.
Once the connection is correctly set up, another rectangle will appear in the home screen, and you'll be able to access Workbench from there.
In this poste, you won't have to set up a connection on your own, as you'll
