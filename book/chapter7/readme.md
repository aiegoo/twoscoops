Table of Contents

7.1 Use get_object_or_404() for Single Objects . . . . . . . . . . . . . . . . 83
7.2 Be Careful With Queries That Might Throw Exceptions . . . . . . . . . 84
7.2.1 ObjectDoesNotExist vs. DoesNotExist . . . . . . . . . . . . . 84
7.2.2 When You Just Want One Object but Get Three Back . . . . . 84
7.3 Use Lazy Evaluation to Make Queries Legible . . . . . . . . . . . . . . 85
7.3.1 Chaining Queries for Legibility . . . . . . . . . . . . . . . . . 86
7.4 Lean on Advanced Query Tools . . . . . . . . . . . . . . . . . . . . . . 87
7.4.1 Query Expressions . . . . . . . . . . . . . . . . . . . . . . . . 88
7.4.2 Database Functions . . . . . . . . . . . . . . . . . . . . . . . . 89
7.5 Don’t Drop Down to Raw SQL Until It’s Necessary . . . . . . . . . . . 90
7.6 Add Indexes as Needed . . . . . . . . . . . . . . . . . . . . . . . . . . 91
7.7 Transactions . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 92
7.7.1 Wrapping Each HTTP Request in a Transaction . . . . . . . . 92
7.7.2 Explicit Transaction Declaration . . . . . . . . . . . . . . . . . 94
7.7.3 django.http.StreamingHttpResponse and Transactions . . . . . 96
7.7.4 Transactions in MySQL . . . . . . . . . . . . . . . . . . . . . 96
7.7.5 Django ORM Transaction Resources . . . . . . . . . . . . . . . 96
7.8 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 97
