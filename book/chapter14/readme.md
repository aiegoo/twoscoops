Table of Contents

```
14.1 Keep Templates Mostly in templates/ . . . . . . . . . . . . . . . . . 173
14.2 Template Architecture Patterns . . . . . . . . . . . . . . . . . . . . . . 174
14.2.1 2-Tier Template Architecture Example . . . . . . . . . . . . . . 174
14.2.2 3-Tier Template Architecture Example . . . . . . . . . . . . . . 174
14.2.3 Flat Is Better Than Nested . . . . . . . . . . . . . . . . . . . . 175
14.3 Limit Processing in Templates . . . . . . . . . . . . . . . . . . . . . . 176
14.3.1 Gotcha 1: Aggregation in Templates . . . . . . . . . . . . . . . 178
14.3.2 Gotcha 2: Filtering With Conditionals in Templates . . . . . . 180
14.3.3 Gotcha 3: Complex Implied Queries in Templates . . . . . . . . 182
14.3.4 Gotcha 4: Hidden CPU Load in Templates . . . . . . . . . . . 183
14.3.5 Gotcha 5: Hidden REST API Calls in Templates . . . . . . . . 183
14.4 Don’t Bother Making Your Generated HTML Pretty . . . . . . . . . . 184
14.5 Exploring Template Inheritance . . . . . . . . . . . . . . . . . . . . . . 185
14.6 block.super Gives the Power of Control . . . . . . . . . . . . . . . . . . 188
14.7 Useful Things to Consider . . . . . . . . . . . . . . . . . . . . . . . . . 189
14.7.1 Avoid Coupling Styles Too Tightly to Python Code . . . . . . . 190
14.7.2 Common Conventions . . . . . . . . . . . . . . . . . . . . . . 190
14.7.3 Use Implicit and Named Explicit Context Objects Properly . . . 190
14.7.4 Use URL Names Instead of Hardcoded Paths . . . . . . . . . . 191
14.7.5 Debugging Complex Templates . . . . . . . . . . . . . . . . . 191
14.8 Error Page Templates . . . . . . . . . . . . . . . . . . . . . . . . . . . 192
14.9 Follow a Minimalist Approach . . . . . . . . . . . . . . . . . . . . . . 193
14.10 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 193

```