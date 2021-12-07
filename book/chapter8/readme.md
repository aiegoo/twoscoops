Table of Contents

8.1 When to Use FBVs or CBVs . . . . . . . . . . . . . . . . . . . . . . . 99
8.2 Keep View Logic Out of URLConfs . . . . . . . . . . . . . . . . . . . 100
8.3 Stick to Loose Coupling in URLConfs . . . . . . . . . . . . . . . . . . 102
8.3.1 What if We Aren’t Using CBVs? . . . . . . . . . . . . . . . . . 104
8.4 Use URL Namespaces . . . . . . . . . . . . . . . . . . . . . . . . . . . 104
8.4.1 Makes for Shorter, More Intuitive, and Don’t Repeat Yourself
URL Names . . . . . . . . . . . . . . . . . . . . . . . . . . . . 106
8.4.2 Increases Interoperability With Third-Party Libraries . . . . . . 106
8.4.3 Easier Searches, Upgrades, and Refactors . . . . . . . . . . . . 108
8.4.4 Allows for More App and Template Reverse Tricks . . . . . . . 108
8.5 Try to Keep Business Logic Out of Views . . . . . . . . . . . . . . . . 108
8.6 Django Views Are Functions . . . . . . . . . . . . . . . . . . . . . . . 108
8.6.1 The Simplest Views . . . . . . . . . . . . . . . . . . . . . . . . 109
8.7 Don’t Use locals() as Views Context . . . . . . . . . . . . . . . . . . 110
8.8 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 111
