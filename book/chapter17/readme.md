Table of Contents

17.1 Fundamentals of Basic REST API Design . . . . . . . . . . . . . . . . 208
17.2 Illustrating Design Concepts With a Simple API . . . . . . . . . . . . 209
17.3 REST API Architecture . . . . . . . . . . . . . . . . . . . . . . . . . . 214
17.3.1 Use Consistent API Module Naming . . . . . . . . . . . . . . 214
17.3.2 Code for a Project Should Be Neatly Organized . . . . . . . . . 215
17.3.3 Code for an App Should Remain in the App . . . . . . . . . . . 215
17.3.4 Try to Keep Business Logic Out of API Views . . . . . . . . . 216
17.3.5 Grouping API URLs . . . . . . . . . . . . . . . . . . . . . . . 217
17.3.6 Test Your API . . . . . . . . . . . . . . . . . . . . . . . . . . . 219
17.3.7 Version Your API . . . . . . . . . . . . . . . . . . . . . . . . . 219
17.3.8 Be Careful With Customized Authentication Schemes . . . . . 219
17.4 When DRF Gets in the Way . . . . . . . . . . . . . . . . . . . . . . . 220
17.4.1 Remote Procedure Calls vs REST APIs . . . . . . . . . . . . . 220
17.4.2 Problems With Complex Data . . . . . . . . . . . . . . . . . . 222
17.4.3 Simplify! Go Atomic! . . . . . . . . . . . . . . . . . . . . . . . 223
17.5 Shutting Down an External API . . . . . . . . . . . . . . . . . . . . . 224
17.5.1 Step #1: Notify Users of Pending Shut Down . . . . . . . . . . 224
17.5.2 Step #2: Replace API With 410 Error View . . . . . . . . . . . 224
17.6 Rate-Limiting Your API . . . . . . . . . . . . . . . . . . . . . . . . . 225
17.6.1 Unfettered API Access Is Dangerous . . . . . . . . . . . . . . . 225
17.6.2 REST Frameworks Must Come With Rate Limiting . . . . . . 226
17.6.3 Rate Limiting Can Be a Business Plan . . . . . . . . . . . . . . 226
17.7 Advertising Your REST API . . . . . . . . . . . . . . . . . . . . . . . 227
17.7.1 Documentation . . . . . . . . . . . . . . . . . . . . . . . . . . 227
17.7.2 Provide Client SDKs . . . . . . . . . . . . . . . . . . . . . . . 227
17.1 Fundamentals of Basic REST API Design . . . . . . . . . . . . . . . . 208
17.2 Illustrating Design Concepts With a Simple API . . . . . . . . . . . . 209
17.3 REST API Architecture . . . . . . . . . . . . . . . . . . . . . . . . . . 214
17.3.1 Use Consistent API Module Naming . . . . . . . . . . . . . . 214
17.3.2 Code for a Project Should Be Neatly Organized . . . . . . . . . 215
17.3.3 Code for an App Should Remain in the App . . . . . . . . . . . 215
17.3.4 Try to Keep Business Logic Out of API Views . . . . . . . . . 216
17.3.5 Grouping API URLs . . . . . . . . . . . . . . . . . . . . . . . 217
17.3.6 Test Your API . . . . . . . . . . . . . . . . . . . . . . . . . . . 219
17.3.7 Version Your API . . . . . . . . . . . . . . . . . . . . . . . . . 219
17.3.8 Be Careful With Customized Authentication Schemes . . . . . 219
17.4 When DRF Gets in the Way . . . . . . . . . . . . . . . . . . . . . . . 220
17.4.1 Remote Procedure Calls vs REST APIs . . . . . . . . . . . . . 220
17.4.2 Problems With Complex Data . . . . . . . . . . . . . . . . . . 222
17.4.3 Simplify! Go Atomic! . . . . . . . . . . . . . . . . . . . . . . . 223
17.5 Shutting Down an External API . . . . . . . . . . . . . . . . . . . . . 224
17.5.1 Step #1: Notify Users of Pending Shut Down . . . . . . . . . . 224
17.5.2 Step #2: Replace API With 410 Error View . . . . . . . . . . . 224
17.6 Rate-Limiting Your API . . . . . . . . . . . . . . . . . . . . . . . . . 225
17.6.1 Unfettered API Access Is Dangerous . . . . . . . . . . . . . . . 225
17.6.2 REST Frameworks Must Come With Rate Limiting . . . . . . 226
17.6.3 Rate Limiting Can Be a Business Plan . . . . . . . . . . . . . . 226
17.7 Advertising Your REST API . . . . . . . . . . . . . . . . . . . . . . . 227
17.7.1 Documentation . . . . . . . . . . . . . . . . . . . . . . . . . . 227
17.7.2 Provide Client SDKs . . . . . . . . . . . . . . . . . . . . . . . 227
