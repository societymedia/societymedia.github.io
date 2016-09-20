---
layout: content
title: Beginning iOS Development using Swift - Day 1
date: 9/20/16
categories: iOS Swift
---

# Welcome to Day One of Improving U - Beginning Xcode with Swift
Today we'll look at Xcode's development environment. We need to __understand__ its UI if we are doing to do anything meaningful in it.  

**XCode is a monster, but can be tamed with this in mind. Learn it on a NEED TO KNOW BASIS**. 

What we are going to do is make sure we get the Prerequisites downloaded or created and then we are going to just touch a few of the areas or panels in XCode.  We will then look at Interface Builder and its different Areas and we'll end the class by using what we learned to start building the UI of our Weather Application by dragging out UI controls onto a Storyboard. So lets get those pesky prerequists out of the way!

### Prerequisites

- XCode 8.0
- An Apple ID
  - Optional Apple Developer Account
- A Weather API Key from developer.forcast.io


### Download Xcode 8.0 from Apple Appstore

This will take some time so lets get that out of the way!

### Apple ID

If you already have an Apple Developer account, you may skip this step. Basically, what we are after is a Free Apple Developer account to use in XCode. All you need is an Apple ID. Go to developer.apple.com, sign in and you're off! If you need to create an Apple ID, you may also do that from the login page. Accept the terms, blah, blah, blah.

#### Link your Apple Developer account to XCode.

Once XCode is downloaded and you have created an AppleID and/or linked it as a Apple Developer Account what we'll want to do is tell XCode about it. 

- In XCode, go to Preferences > Accounts and click the '+' in the bottom. Login using your AppleID.

### Create an Account on forcast.io

We'll be using the forcast.io API to get weather for our app. So go to developer.forcast.io and create an account.

### XCode IDE

Once you have XCode 8.0 installed and an AppleId linked inside XCode, you are ready to start building our Weather Application..

### **REMEMBER: Take the Learning of Xcode on a 'Need to know Basis'**

XCode is an IDE that includes everything you need to create an app. Its separated by different Areas to help you organize and edit your code, build, debug and run your app.
Lets first use XCode and create our Weather Application. 
 
- Open XCode and 'Create a new XCode project'
- Choose 'Single View Application'

#### In the Next Dialog that appears

- Product Name: Xcode uses the product name you entered to name your project and the app.
- Organization Name: The name of your organization or your own name. You can leave this blank.
- Organization Identifier: Your organization identifier, if you have one. If you don’t, use com.example.
- Bundle Identifier: This value is automatically generated based on your product name and organization identifier.
- Language: Swift
- Devices: Choose iPhone but know that 'Universal' is what is used when you want your app to run on an iPhone AND iPad
- Use Core Data: leave this Unselected.
- Include Unit Tests: leave this Unselected.
- Include UI Tests: leave this Unselected.

#### Now we have our Weather Application.

### Workspace Window

---



In the workspace window, you may or may not see a warning triangle with a message that says “No code signing identities found.” 
Click the fix it and select the account you used earlier. 

Lets take a few minutes to help familiarize yourself with some of the main Areas of XCode

### Toolbar

----

#### Run button - Clicking this button instructs Xcode to compile and run our application in either the iOS simulator or on a connected iPhone.

Additionally, if you click and hold this button, you can change it from Run to another action, such as Test, Profile, or Analyze. 

- The Test action runs any unit tests that you have set up
- The Profile action runs the application Instruments
- The Analyze action checks your code and points out potential problems and bugs.

#### Stop button

Clicking this button stops any task that Xcode is currently doing—if it’s building your application, it stops; and if your application is running in the debugger, it quits it.

#### Scheme Selector

Schemes are what Xcode calls build configurations—that is, what’s being built, how, and where it will run. This is where you can change it from an iOS Simulator or a selected iOS Device

#### Status display

The status display shows what Xcode is doing—building your application, downloading documentation, installing an application on an iOS device, and so on.

#### Editor selector

The editor selector determines how the editor is laid out. You can choose to display either a single editor, the editor with the assistant, or the versions editor, which allows you to compare different versions of a file if you’re using a revision control system like Git or Subversion.

#### View selector

The view selector controls whether the navigator, debug, and utility panes appear on screen. If you’re pressed for screen space or simply want less clutter, you can quickly summon and dismiss these parts of the screen by clicking each of the elements.

### Navigator Area

----

The navigator Area is separated by the icons on the top.

#### Project navigator

Lists all the files that make up your project. This is the most commonly used navigator, as it determines what is shown in the editor. Whatever is selected in the project navigator is opened in the editor.

#### Symbol navigator

Lists all the classes and functions that exist in your project. If you’re looking for a quick summary of a class or want to jump directly to a method in that class, the symbol navigator is a handy tool.

#### Search navigator

Allows you to perform searches across your project if you’re looking for specific text. (The shortcut is ⌘-Shift-F. Press ⌘-F to search the current open document.)

#### Issue navigator

Lists all the problems that Xcode has noticed in your code. This includes warnings, compilation errors, and issues that the built-in code analyzer has spotted.

#### Test navigator

Shows all the unit tests associated with your project. Unit tests used to be an optional component of Xcode but are now built into Xcode directly.

#### Debug navigator

Activated when you’re debugging a program, and it allows you to examine the state of the various threads that make up your program.

#### Breakpoint navigator

Lists all of the breakpoints that you’ve set for use while debugging.

#### Report navigator

Lists all the activity that Xcode has done with your project (such as building, debugging, and analyzing). You can go back and view previous build reports from earlier in your Xcode session, too.

### Editor Area

----

The XCode editor is where you’ll be spending most of your time. This is where you be doing things like

- Source code editing
- Interface design, 
- Project configuration

If you’re editing source code, the editor is a text editor, with code completion, syntax highlighting, and all the usual features that developers have come to expect from an integrated development environment. If you’re modifying a user interface, the editor becomes a visual editor, allowing you to drag around the components of your interface. Other kinds of files have their own specialized editors as well.

At the top of the editor, you’ll find the jump bar. The jump bar lets you quickly jump from the content that you’re editing to another piece of related content, such as a file in the same folder. The jump bar is a fast way to navigate your project.

### Utility Area ###

----

The utilities pane shows additional information related to what you’re doing in the editor. Its contextual so if you’re editing a Swift source file, for example, the utilities pane allows you to view and modify settings for that file.

### Debug Area

----

The debug area shows information reported by the debugger when the program is running. Whenever you want to see what the application is reporting while running, you can view it in the debug area. By default the debug area is not shown unless there is a program running. You can bring up the debug area by using the Xcode Toolbar View selector middle button.

The area is split into two sections: the left hand side shows the values of local variables when the application is paused; the right hand side shows the ongoing log from the debugger, which includes any logging that comes from the debugged application.

### Interface Builder

----

### Designing the Interface

When building any UI, you have two options. 

- Declarative using a storyboard
- Pragmatically using source code

As a general rule, storyboards are a better way to create your interfaces as it shows you how all the screens link together.

Start by opening the main.storyboard. Then buy a great big monitor.
Lets use our XCode chops to help maximize our workspace by collapsing Areas we don't need now.

Next, lets spend some more time familiarizing ourselves with Interface Builder.

#### Document Outline

This is the area you will use to help navigate your scenes. Each Scene is basically a 'View' in an Application. Each 'View' is composed of one or more UI Controls and accessible from the Document Outline.


#### Editor Area

While viewing a .storyboard file the editor area will give you a high level view of your screens.

#### Utilities Area

Make sure your Utilities Area is visible by clicking on appropriate View Selector.
All user interface controls are kept in the Object library, which is at the bottom of the utilities pane on the right hand side of the screen.

#### Lets Go!

Lets spend the rest of the class designing our UI together. Rather than me deciding how our application should flow, I'll help guide us down the path with a few guidelines and Controls needed in subsequent classes. We need to also keep in mind that our Application should change depending on our Application's orientation: Landscape or Portrait.

- Need a UINavigationController
- Need either a UITableViewController or UITableView
- UIBarButtons
- UI to fetch weather by longitude and latitude (UITextFields and UIButton)
- A Scene to view Forcast Details
- UIImageView
- UILabels
- MKMapView

Lets put or Microsoft Developer hats on start dragging!             

#### Object Library

Using the Object library, which is at the bottom of the utilities pane on the right hand side of the screen lets find controls, using the search field, and drag them on our scene.

####Configure a UI Control.

Every control that you add to the storyboard can be configured using the Utilities area, remembering the Utilities area is contextual 

#### Attributes Inspector

Select the control by either clicking it on the storyboard or clicking on it in the document outline, then and select the Attributes Inspector, which is the third tab from the right at the top of the utilities pane. You can also reach it by pressing ⌘-Option-4.

There are many attributes on control;

#### Segues

Segues allow us to define the flow of our application. It defines a relationship between two controllers in the storyboard and how one screen transitions to another screen

#### Create *Controllers for our Scenes

Applications aren’t just interfaces—as a developer, you also need to write code. To work with the interface you’ve designed, you need to create connections between your code and your interface.

#### Connecting the Code

There are three kinds of connections that you can make. We will only talk about 2 of them:

- Outlets
- Actions 

Outlines are variables that refer to objects in the interface. Using outlets, you can instruct a button to change color or size, or to hide itself.
Actions are methods in your code that are run in response to the user interacting with an object. These interactions include the user touching a finger to an object, dragging a finger, and so on.



