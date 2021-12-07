Table of Contents

6.1 Basics . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 63
6.1.1 Break Up Apps With Too Many Models . . . . . . . . . . . . . 63
6.1.2 Be Careful With Model Inheritance . . . . . . . . . . . . . . . 64
6.1.3 Model Inheritance in Practice: The TimeStampedModel . . . . 65
6.2 Database Migrations . . . . . . . . . . . . . . . . . . . . . . . . . . . . 67
6.2.1 Tips for Creating Migrations . . . . . . . . . . . . . . . . . . . 67
6.2.2 Adding Python Functions and Custom SQL to Migrations . . . 67
6.3 Overcoming Common Obstacles of RunPython . . . . . . . . . . . . . 68
6.3.1 Getting Access to a Custom Model Manager’s Methods . . . . . 68
6.3.2 Getting Access to a Custom Model Method . . . . . . . . . . . 68
6.3.3 Use RunPython.noop to Do Nothing . . . . . . . . . . . . . . 68
6.3.4 Deployment and Management of Migrations . . . . . . . . . . 70
6.4 Django Model Design . . . . . . . . . . . . . . . . . . . . . . . . . . . 70
6.4.1 Start Normalized . . . . . . . . . . . . . . . . . . . . . . . . . 71
6.4.2 Cache Before Denormalizing . . . . . . . . . . . . . . . . . . . 71
6.4.3 Denormalize Only if Absolutely Needed . . . . . . . . . . . . . 71
6.4.4 When to Use Null and Blank . . . . . . . . . . . . . . . . . . . 71
6.4.5 When to Use BinaryField . . . . . . . . . . . . . . . . . . . . . 72
6.4.6 Try to Avoid Using Generic Relations . . . . . . . . . . . . . . 74
6.4.7 Make Choices and Sub-Choices Model Constants . . . . . . . . 75
6.4.8 Using Enumeration Types for Choices . . . . . . . . . . . . . . 76
6.4.9 PostgreSQL-Specific Fields: When to Use Null and Blank . . . 77
6.5 The Model _meta API . . . . . . . . . . . . . . . . . . . . . . . . . . 77
6.6 Model Managers . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 78
6.7 Understanding Fat Models . . . . . . . . . . . . . . . . . . . . . . . . 80
6.7.1 Model Behaviors a.k.a Mixins . . . . . . . . . . . . . . . . . . 81
6.7.2 Stateless Helper Functions . . . . . . . . . . . . . . . . . . . . 81
6.7.3 Model Behaviors vs Helper Functions . . . . . . . . . . . . . . 81
6.8 Additional Resources . . . . . . . . . . . . . . . . . . . . . . . . . . . 81
6.9 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 82
