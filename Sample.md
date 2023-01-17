Consider that you are working on an essay for school. Initially, you will create a draft and save it in your system, now after completing the initial draft you made some changes like adding new information, deleting irrelevant information and correcting grammatical errors in the file. After making all these changes you will save the document using save as and save it as draft 2. You might be thinking why should I replace the draft one with the updated draft?

The reason might be that the verbose in the initial draft might be better or the information that you deleted might be important. So it's better to save the file as draft two.  Now consider it is a folder with multiple files, It becomes complex to store multiple drafts of all the files in the folder, Now consider that it's a group assignment and multiple people are working on the same files. Now it becomes even more complex.  After a while, it becomes hard to figure out which file contains what information and what changes were made.

Now let's correlate this example for software development. Similar to draft one and draft two, for every application launched, we have semantic versioning. A public API should be declared and the changes can be communicated to the API by incrementing the version number.  Semantic versioning contains three major indicators called Major, Minor and patch, represented as `Major.Minor.Patch`.  This number doesn't represent the size of the software or application.

Let's consider an initial release of a drone 1.0.0

It has some basic functionalities:


```
Move Up/Down (Throttle)
Tilt Forward/Backward (Pitch)
Move Left/Right ( Roll)
```


Everything looks fine but A Dorne itself is not worth more than a toy, to add some additional functionality a camera is added to the drone. 

Now the version is 1.1.0

```
Move Up/Down (Throttle)
Tilt Forward/Backward (Pitch)
Move Left/Right ( Roll)
Camera
```

This addition of the camera is a minor update because even without the camera the drone works but it's preferred to have a camera attached to the drone. Based on this example it can be concluded that the minor update brings a new feature which changes the API but is backwards compatible. To simply define, the minor update is a non-breakable change.

To improve the visibility and ease of image capturing a new movement should be added to rotate the drone left or right called Yaw. this upgradation is called a patch. Patch updates are interchangeable and consumers should update their software without hesitation. 


1.1.1

```
Move Up/Down (Throttle)
Tilt Forward/Backward (Pitch)
Move Left/Right ( Roll)
Camera
Rotate  Left/Right ( Roll )
```

Now consider that The purpose of the drone is changed and now the drone is used to spray pesticides instead of image capturing.

The new update is 2.0.0


```
Move Up/Down (Throttle)
Tilt Forward/Backward (Pitch)
Move Left/Right ( Roll)
Rotate  Left/Right ( Roll )
Camera
Storage tank and spray equipment.
```

The above update will change the software. The camera is removed and a new updated storage tank and spray equipment is added.
The major update will cause interface change and breaks the backward compatibility.


The above versioning applies to software development. As the number of updates grows, it becomes hard to classify and manage all the versions. On top of that the real-life development process includes collaboration. When multiple people work on the same project consisting of multiple files, it will lead to the following issues will arise:

1. Storage: All the files created for all changes will take up more storage.
2. Tracking: multiple changes made by multiple collaborators should be tracked.
3. Maintenance: The changes if not tested properly may break the application and if that happens the application must revert to its recent stable version.
4. Security: Not everyone should be allowed to make changes to the application.

To solve all the above problems and to add some additional functionalities version control system is used.

for aditional information refer [semver](https://semver.org/)

Version Control System:

Version control system are classified into two types, they are

Centralized
Distributed

Consider a scenario where one of your friends has a borad game and in order to lay that game, all the friends can access it from that specific friend. This is an example for centralized VCS and now consider that a group of friends are playing an online game. Insted of gathering at a single palce all the friends can connect and play from ther home. This is an example for dsistributed VCS.

To put it in technical terms, centralized VSC has a single central copy of project and programmers will access and commit their chnages form that copy. This arrangement is not prefered because if the central sever fails, the entire project fails. few examples for centralized VCS are  CVS Preforce and subversion.


image

In distributed VCS the codebase maintained in the server is coppied to every individual developers system. Even though a single user looses the data or a failure occurs in sungle system, the code is preserved. Few examples for distributed VCS are GIT and Mecurial.

image



for additional information refer the document [VCS](https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control)

GIT :

As explained GIT is  a free and opensource distributed version control system. It is used to handle small to larg projects with speed and efficiency.

To install GIT refere the document [Git download](https://git-scm.com/downloads)

Once the installation procedure is completed, to check if GIT is installed in you system run the following command in the command prompt(windows) or terminal in caseof mac os or linix.

``` git
 git --version
```

If git is installed, the output  should be the git version installed in your system.

GIT can be accessed using command line, IDE and GUI.  In this documnt we will use commad line(Git Bash) and Visual Studio IDE. 
