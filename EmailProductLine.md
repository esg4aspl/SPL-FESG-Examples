# Email Product Line 

Email product line has 5 features and a core feature. 

Remember that the core of the product line represents the common behavior which exists in all products that belong to Email Product Line. The core behavior is modelled using core ESG (c-ESG).An optional behavior is modelled using a feature ESG (f-ESG). 

## Feature Model

![Feature Model](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailPL_ModelImages/EmailPL_featureModel.PNG)\
This feature model has 5 optional features. The features _encrypt_ and _forward_ cannot belong to the same product at the same time. 24 different product configurations could be obtained by combining these features of the feature model.

## Email Products
There are 24 product configurations in Email Product Line. In the table below, the product id and the belonging features are given. Since, each possible product does not have a unique official name, we assign IDs to products to name them uniquely.

| Product ID | Features                                  |
| ---------- | ----------------------------------------- |
| 0          | \-                                        |
| 1          | addressbook                               |
| 2          | autoresponder                             |
| 4          | forward                                   |
| 8          | encrypt                                   |
| 12         | sign                                      |
| 3          | addressbook, autoresponder                |
| 5          | addressbook, forward                      |
| 6          | autoresponder, forward                    |
| 9          | addressbook, encrypt                      |
| 10         | autoresponder, encrypt                    |
| 13         | addressbook, sign                         |
| 14         | autoresponder, sign                       |
| 16         | forward, sign                             |
| 20         | encrypt, sign                             |
| 7          | addressbook, autoresponder, forward       |
| 11         | addressbook, autoresponder, encrypt       |
| 15         | addressbook, autoresponder, sign          |
| 17         | addressbook, forward, sign                |
| 18         | autoresponder, forward, sign              |
| 21         | addressbook, encrypt, sign                |
| 22         | autoresponder, encrypt, sign              |
| 19         | addressbook, autoresponder, forward, sign |
| 23         | addressbook, autoresponder, encrypt, sign |

# Email Product Line Features
## Core ESG (c-ESG)
 ![core](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailPL_ModelImages/core.PNG)\
 The core ESG of the elevator product line represents core features, which exist in all product configurations. For this product line the core feature is composing a new email, sending an email and receiving an email. Note that, the product that has the ID 0, has only core feature since the core feature itself, is capable of generating test sequences.\
 [Core ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailPL_Models/core.zip)

## Addressbook Feature ESG (f-ESG)
![addressbook](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailPL_ModelImages/addressbook.PNG)\
Addressbook feature helps a user to create an addressbook for a contact who has more than one email address and to send an email to all of the contact's email addresses.\
[Addressbook Feature ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailPL_Models/addressbook.zip)

## Autoresponder Feature ESG (f-ESG)
![autoresponder](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailPL_ModelImages/autoresponder.PNG)\
Autoresponder feature helps the user to compose a autoresponse email body and set the date interval of autoresponse.\
[Autoresponder Feature ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailPL_Models/autoresponder.zip)

## Forward Feature ESG (f-ESG)
![forward](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailPL_ModelImages/forward.PNG)\
Forward activates the email account's forwarding email feature. \
[Forward Feature ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailPL_Models/forward.zip)

## Encrypt Feature ESG (f-ESG)
![encrypt](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailPL_ModelImages/encrypt.PNG)\
Encrypt feature helps the user to encrypt the sending email.\
[Encrypt Feature ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailPL_Models/encrypt.zip)

## Sign Feature ESG (f-ESG)
![sign](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailPL_ModelImages/sign.PNG)\
Sign feature adds sender's signature to the email.\
[Sign Feature ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailPL_Models/sign.zip)
[Click to download all ESG MXE Files](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailPL_Models/EmailPL_Models.zip)

# Email Product Line Test Generation and Execution
The Email Product Line has 24 product configurations and 52 one-increment, i.e., one feature addition, testing scenarios in total. In our study, we select 30 of the testing scenarios randomly. In the selection process of the one increment scenarios, the following two rules are applied:
1.	The same scenario has not been selected more than once.	
2.	The same PUC has not been selected more than twice.

## Testing Scenarios
In this table, the selected testing scenarios are given with their Scenario IDs, Product Under Consideration(PUC) IDs, Existing Product IDs and Features and Increment. Existing Product refers to the product that we already have the model and the test sequences. In incremental test generation approach, the existing product's test sequences and increment's test sequences are composed so that the test sequences of the PUC is obtained without generating and composing all of its features from scratch. 

| Scenario ID | Product Under Consideration ID | Existing Product ID | Existing Product Features           | Increment     |
| ----------- | ------------------------------ | ------------------- | ----------------------------------- | ------------- |
| 1           | 2                              | 0                   | \-                                  | autoresponder |
| 2           | 4                              | 0                   | \-                                  | forward       |
| 3           | 8                              | 0                   | \-                                  | encrypt       |
| 4           | 12                             | 0                   | \-                                  | sign          |
| 5           | 3                              | 1                   | addressbook                         | autoresponder |
| 6           | 5                              | 1                   | addressbook                         | forward       |
| 7           | 9                              | 1                   | addressbook                         | encrypt       |
| 8           | 13                             | 1                   | addressbook                         | sign          |
| 9           | 3                              | 2                   | autoresponder                       | addressbook   |
| 14          | 11                             | 3                   | addressbook, autoresponder          | encrypt       |
| 18          | 16                             | 4                   | forward                             | sign          |
| 19          | 7                              | 5                   | addressbook, forward                | autoresponder |
| 21          | 7                              | 6                   | autoresponder, forward              | addressbook   |
| 23          | 19                             | 7                   | addressbook, autoresponder, forward | sign          |
| 26          | 20                             | 8                   | encrypt                             | sign          |
| 27          | 11                             | 9                   | addressbook, encrypt                | autoresponder |
| 28          | 21                             | 9                   | addressbook, encrypt                | sign          |
| 30          | 22                             | 10                  | autoresponder, encrypt              | sign          |
| 31          | 23                             | 11                  | addressbook, autoresponder, encrypt | sign          |
| 33          | 14                             | 12                  | sign                                | autoresponder |
| 34          | 16                             | 12                  | sign                                | forward       |
| 35          | 20                             | 12                  | sign                                | encrypt       |
| 36          | 15                             | 13                  | addressbook, sign                   | autoresponder |
| 39          | 15                             | 14                  | autoresponder, sign                 | addressbook   |
| 40          | 18                             | 14                  | autoresponder, sign                 | forward       |
| 45          | 18                             | 16                  | forward, sign                       | autoresponder |
| 47          | 19                             | 18                  | autoresponder, forward, sign        | addressbook   |
| 48          | 21                             | 20                  | encrypt, sign                       | addressbook   |
| 49          | 22                             | 20                  | encrypt, sign                       | autoresponder |
| 51          | 23                             | 22                  | autoresponder, encrypt, sign        | addressbook   |

## Data on PUC
The numbers of k-sequences where k=1,2,3,4 are given to give a notion of the sizes of the selected PUCs in the testing scenarios.

| Product Under Consideration ID | k = 1 |  k = 2 | k = 3 | k = 4 |
| ------------------------------ | ----- | ------ | ----- | ----- |
| 2                              | 9     | 15     | 35    | 89    |
| 3                              | 13    | 19     | 41    | 104   |
| 4                              | 8     | 15     | 35    | 88    |
| 5                              | 12    | 19     | 41    | 103   |
| 7                              | 14    | 21     | 43    | 105   |
| 8                              | 9     | 16     | 39    | 103   |
| 9                              | 13    | 20     | 45    | 118   |
| 11                             | 15    | 22     | 47    | 120   |
| 12                             | 8     | 15     | 38    | 102   |
| 13                             | 12    | 19     | 44    | 117   |
| 14                             | 10    | 17     | 40    | 104   |
| 15                             | 14    | 21     | 46    | 119   |
| 16                             | 9     | 17     | 40    | 103   |
| 18                             | 11    | 19     | 42    | 105   |
| 19                             | 15    | 23     | 48    | 120   |
| 20                             | 10    | 18     | 44    | 118   |
| 21                             | 14    | 22     | 50    | 133   |
| 22                             | 12    | 20     | 46    | 120   |
| 23                             | 16    | 24     | 52    | 135   |

## Data on Number of Faults
The table below contains the total number of possible faults and the number of faults seeded for various m values for each PUC. The entire number of possible faults for each PUC for a given value of m is directly proportional to the number of m-sequences in the PUC's ESG, and the total number of seeded faults is 20% of the summation of number of possible faults for m=2,3,4,5.

| Scenario ID | PUC ID | m=2 | m=3 | m=4 | m=5 | Number of Seeded Faults |
| ----------- | ------ | --- | --- | --- | --- | ----------------------- |
| 1           | 2      | 24  | 50  | 124 | 319 | 103                     |
| 2           | 4      | 23  | 50  | 123 | 316 | 102                     |
| 3           | 8      | 25  | 55  | 142 | 375 | 119                     |
| 4           | 12     | 23  | 53  | 140 | 370 | 117                     |
| 5           | 3      | 32  | 60  | 145 | 374 | 122                     |
| 6           | 5      | 31  | 60  | 144 | 371 | 121                     |
| 7           | 9      | 33  | 65  | 163 | 430 | 138                     |
| 8           | 13     | 31  | 63  | 161 | 425 | 136                     |
| 9           | 3      | 32  | 60  | 145 | 374 | 122                     |
| 14          | 11     | 37  | 69  | 167 | 434 | 141                     |
| 18          | 16     | 26  | 57  | 143 | 371 | 119                     |
| 19          | 7      | 35  | 64  | 148 | 375 | 124                     |
| 21          | 7      | 35  | 64  | 148 | 375 | 124                     |
| 23          | 19     | 38  | 71  | 168 | 430 | 141                     |
| 26          | 20     | 28  | 62  | 162 | 430 | 136                     |
| 27          | 11     | 37  | 69  | 167 | 434 | 141                     |
| 28          | 21     | 36  | 72  | 183 | 485 | 155                     |
| 30          | 22     | 32  | 66  | 166 | 434 | 140                     |
| 31          | 23     | 40  | 76  | 187 | 489 | 158                     |
| 33          | 14     | 27  | 57  | 144 | 374 | 120                     |
| 34          | 16     | 26  | 57  | 143 | 371 | 119                     |
| 35          | 20     | 28  | 62  | 162 | 430 | 136                     |
| 36          | 15     | 35  | 67  | 165 | 429 | 139                     |
| 39          | 15     | 35  | 67  | 165 | 429 | 139                     |
| 40          | 18     | 30  | 61  | 147 | 375 | 123                     |
| 45          | 18     | 30  | 61  | 147 | 375 | 123                     |
| 47          | 19     | 38  | 71  | 168 | 430 | 141                     |
| 48          | 21     | 36  | 72  | 183 | 485 | 155                     |
| 49          | 22     | 32  | 66  | 166 | 434 | 140                     |
| 51          | 23     | 40  | 76  | 187 | 489 | 158                     |

## Data on Test Generation and Execution
Table below presents data on fault coverage and performance statistics on test set generation and test execution processes.

| Scenario ID | PUC ID | Test Set | Existing Product Number of Sequences | Existing Product Number of Events | PUC Number of Sequences | PUC Number of Events | Number of Common Sequences | Number of Common Events | Generation Time | Faults Seeded | Events Executed | Faults Revealed |
| ----------- | ------ | -------- | ------------------------------------ | --------------------------------- | ----------------------- | -------------------- | -------------------------- | ----------------------- | --------------- | ------------- | --------------- | --------------- |
| 1           | 2      | inc(2)   | 4                                    | 20                                | 6                       | 25                   | 4                          | 20                      | 1.50            | 103           | 192             | 47              |
| 1           | 2      | sm(2)    | \-                                   | \-                                | 6                       | 25                   | \-                         | \-                      | 52.64           | 103           | 190             | 47              |
| 1           | 2      | inc(3)   | 10                                   | 61                                | 13                      | 69                   | 6                          | 37                      | 2.35            | 103           | 363             | 69              |
| 1           | 2      | sm(3)    | \-                                   | \-                                | 12                      | 68                   | \-                         | \-                      | 62.78           | 103           | 373             | 69              |
| 1           | 2      | inc(4)   | 26                                   | 185                               | 30                      | 197                  | 18                         | 131                     | 5.05            | 103           | 628             | 89              |
| 1           | 2      | sm(4)    | \-                                   | \-                                | 27                      | 192                  | \-                         | \-                      | 89.96           | 103           | 603             | 86              |
| 2           | 4      | inc(2)   | 4                                    | 20                                | 5                       | 24                   | 4                          | 20                      | 1.58            | 102           | 182             | 45              |
| 2           | 4      | sm(2)    | \-                                   | \-                                | 5                       | 24                   | \-                         | \-                      | 54.07           | 102           | 180             | 45              |
| 2           | 4      | inc(3)   | 10                                   | 61                                | 11                      | 65                   | 8                          | 49                      | 3.98            | 102           | 374             | 66              |
| 2           | 4      | sm(3)    | \-                                   | \-                                | 11                      | 65                   | \-                         | \-                      | 62.11           | 102           | 351             | 67              |
| 2           | 4      | inc(4)   | 26                                   | 185                               | 27                      | 189                  | 22                         | 154                     | 6.41            | 102           | 620             | 86              |
| 2           | 4      | sm(4)    | \-                                   | \-                                | 26                      | 187                  | \-                         | \-                      | 93.38           | 102           | 610             | 86              |
| 3           | 8      | inc(2)   | 4                                    | 20                                | 5                       | 27                   | 4                          | 20                      | 1.95            | 119           | 215             | 45              |
| 3           | 8      | sm(2)    | \-                                   | \-                                | 4                       | 22                   | \-                         | \-                      | 53.00           | 119           | 220             | 46              |
| 3           | 8      | inc(3)   | 10                                   | 61                                | 15                      | 89                   | 8                          | 49                      | 6.52            | 119           | 484             | 79              |
| 3           | 8      | sm(3)    | \-                                   | \-                                | 11                      | 72                   | \-                         | \-                      | 63.49           | 119           | 474             | 78              |
| 3           | 8      | inc(4)   | 26                                   | 185                               | 48                      | 357                  | 21                         | 152                     | 32.31           | 119           | 942             | 109             |
| 3           | 8      | sm(4)    | \-                                   | \-                                | 29                      | 223                  | \-                         | \-                      | 106.41          | 119           | 791             | 104             |
| 4           | 12     | inc(2)   | 4                                    | 20                                | 5                       | 26                   | 4                          | 20                      | 2.20            | 117           | 220             | 46              |
| 4           | 12     | sm(2)    | \-                                   | \-                                | 4                       | 21                   | \-                         | \-                      | 52.80           | 117           | 222             | 46              |
| 4           | 12     | inc(3)   | 10                                   | 61                                | 15                      | 94                   | 8                          | 49                      | 7.00            | 117           | 516             | 82              |
| 4           | 12     | sm(3)    | \-                                   | \-                                | 11                      | 68                   | \-                         | \-                      | 63.20           | 117           | 474             | 79              |
| 4           | 12     | inc(4)   | 26                                   | 185                               | 44                      | 297                  | 22                         | 155                     | 25.54           | 117           | 809             | 105             |
| 4           | 12     | sm(4)    | \-                                   | \-                                | 29                      | 211                  | \-                         | \-                      | 99.53           | 117           | 742             | 101             |
| 5           | 3      | inc(2)   | 6                                    | 29                                | 8                       | 34                   | 6                          | 29                      | 1.23            | 122           | 216             | 51              |
| 5           | 3      | sm(2)    | \-                                   | \-                                | 7                       | 29                   | \-                         | \-                      | 52.83           | 122           | 209             | 51              |
| 5           | 3      | inc(3)   | 15                                   | 88                                | 18                      | 96                   | 13                         | 76                      | 2.47            | 122           | 471             | 81              |
| 5           | 3      | sm(3)    | \-                                   | \-                                | 14                      | 78                   | \-                         | \-                      | 67.54           | 122           | 448             | 80              |
| 5           | 3      | inc(4)   | 39                                   | 264                               | 43                      | 283                  | 25                         | 163                     | 3.46            | 122           | 815             | 111             |
| 5           | 3      | sm(4)    | \-                                   | \-                                | 32                      | 223                  | \-                         | \-                      | 87.86           | 122           | 777             | 107             |
| 6           | 5      | inc(2)   | 6                                    | 29                                | 7                       | 33                   | 6                          | 29                      | 0.76            | 121           | 244             | 55              |
| 6           | 5      | sm(2)    | \-                                   | \-                                | 6                       | 28                   | \-                         | \-                      | 56.40           | 121           | 232             | 54              |
| 6           | 5      | inc(3)   | 15                                   | 85                                | 16                      | 89                   | 13                         | 73                      | 1.50            | 121           | 460             | 83              |
| 6           | 5      | sm(3)    | \-                                   | \-                                | 13                      | 75                   | \-                         | \-                      | 63.91           | 121           | 439             | 80              |
| 6           | 5      | inc(4)   | 39                                   | 261                               | 40                      | 264                  | 29                         | 189                     | 2.43            | 121           | 806             | 109             |
| 6           | 5      | sm(4)    | \-                                   | \-                                | 31                      | 218                  | \-                         | \-                      | 93.69           | 121           | 764             | 107             |
| 7           | 9      | inc(2)   | 6                                    | 29                                | 7                       | 36                   | 6                          | 29                      | 0.83            | 138           | 313             | 66              |
| 7           | 9      | sm(2)    | \-                                   | \-                                | 5                       | 26                   | \-                         | \-                      | 51.34           | 138           | 315             | 64              |
| 7           | 9      | inc(3)   | 15                                   | 87                                | 22                      | 141                  | 10                         | 55                      | 4.67            | 138           | 621             | 99              |
| 7           | 9      | sm(3)    | \-                                   | \-                                | 14                      | 87                   | \-                         | \-                      | 60.61           | 138           | 556             | 96              |
| 7           | 9      | inc(4)   | 40                                   | 261                               | 60                      | 400                  | 31                         | 200                     | 26.15           | 138           | 1045            | 128             |
| 7           | 9      | sm(4)    | \-                                   | \-                                | 37                      | 271                  | \-                         | \-                      | 97.76           | 138           | 929             | 124             |
| 8           | 13     | inc(2)   | 6                                    | 29                                | 7                       | 35                   | 6                          | 29                      | 0.76            | 136           | 286             | 62              |
| 8           | 13     | sm(2)    | \-                                   | \-                                | 5                       | 25                   | \-                         | \-                      | 51.92           | 136           | 241             | 55              |
| 8           | 13     | inc(3)   | 15                                   | 85                                | 21                      | 119                  | 13                         | 73                      | 4.17            | 136           | 558             | 99              |
| 8           | 13     | sm(3)    | \-                                   | \-                                | 14                      | 83                   | \-                         | \-                      | 62.83           | 136           | 585             | 97              |
| 8           | 13     | inc(4)   | 40                                   | 261                               | 57                      | 373                  | 28                         | 180                     | 21.28           | 136           | 967             | 121             |
| 8           | 13     | sm(4)    | \-                                   | \-                                | 37                      | 259                  | \-                         | \-                      | 99.04           | 136           | 844             | 115             |
| 9           | 3      | inc(2)   | 6                                    | 25                                | 8                       | 34                   | 6                          | 25                      | 2.71            | 122           | 216             | 51              |
| 9           | 3      | sm(2)    | \-                                   | \-                                | 7                       | 29                   | \-                         | \-                      | 52.83           | 122           | 209             | 51              |
| 9           | 3      | inc(3)   | 13                                   | 69                                | 19                      | 97                   | 9                          | 45                      | 7.59            | 122           | 478             | 85              |
| 9           | 3      | sm(3)    | \-                                   | \-                                | 14                      | 78                   | \-                         | \-                      | 67.54           | 122           | 448             | 80              |
| 9           | 3      | inc(4)   | 30                                   | 197                               | 49                      | 312                  | 22                         | 141                     | 7.67            | 122           | 842             | 113             |
| 9           | 3      | sm(4)    | \-                                   | \-                                | 32                      | 223                  | \-                         | \-                      | 87.86           | 122           | 777             | 107             |
| 14          | 11     | inc(2)   | 8                                    | 34                                | 9                       | 41                   | 8                          | 34                      | 0.88            | 141           | 296             | 69              |
| 14          | 11     | sm(2)    | \-                                   | \-                                | 7                       | 31                   | \-                         | \-                      | 52.08           | 141           | 298             | 68              |
| 14          | 11     | inc(3)   | 18                                   | 91                                | 23                      | 121                  | 15                         | 74                      | 4.53            | 141           | 547             | 96              |
| 14          | 11     | sm(3)    | \-                                   | \-                                | 16                      | 94                   | \-                         | \-                      | 63.38           | 141           | 493             | 96              |
| 14          | 11     | inc(4)   | 44                                   | 275                               | 68                      | 473                  | 34                         | 206                     | 21.45           | 141           | 1045            | 129             |
| 14          | 11     | sm(4)    | \-                                   | \-                                | 39                      | 280                  | \-                         | \-                      | 130.03          | 141           | 961             | 123             |
| 18          | 16     | inc(2)   | 4                                    | 22                                | 5                       | 28                   | 4                          | 22                      | 0.92            | 119           | 205             | 46              |
| 18          | 16     | sm(2)    | \-                                   | \-                                | 5                       | 25                   | \-                         | \-                      | 57.14           | 119           | 179             | 42              |
| 18          | 16     | inc(3)   | 10                                   | 63                                | 15                      | 94                   | 8                          | 51                      | 3.84            | 119           | 446             | 81              |
| 18          | 16     | sm(3)    | \-                                   | \-                                | 12                      | 72                   | \-                         | \-                      | 64.84           | 119           | 388             | 76              |
| 18          | 16     | inc(4)   | 26                                   | 187                               | 41                      | 279                  | 19                         | 138                     | 32.35           | 119           | 802             | 109             |
| 18          | 16     | sm(4)    | \-                                   | \-                                | 30                      | 215                  | \-                         | \-                      | 139.84          | 119           | 754             | 106             |
| 19          | 7      | inc(2)   | 6                                    | 31                                | 8                       | 36                   | 6                          | 31                      | 1.20            | 124           | 213             | 53              |
| 19          | 7      | sm(2)    | \-                                   | \-                                | 8                       | 33                   | \-                         | \-                      | 55.59           | 124           | 210             | 53              |
| 19          | 7      | inc(3)   | 15                                   | 85                                | 18                      | 98                   | 11                         | 63                      | 2.64            | 124           | 476             | 85              |
| 19          | 7      | sm(3)    | \-                                   | \-                                | 15                      | 82                   | \-                         | \-                      | 65.86           | 124           | 462             | 83              |
| 19          | 7      | inc(4)   | 40                                   | 265                               | 43                      | 280                  | 31                         | 206                     | 3.66            | 124           | 788             | 110             |
| 19          | 7      | sm(4)    | \-                                   | \-                                | 33                      | 227                  | \-                         | \-                      | 92.83           | 124           | 762             | 110             |
| 21          | 7      | inc(2)   | 6                                    | 27                                | 8                       | 36                   | 6                          | 27                      | 1.07            | 124           | 213             | 53              |
| 21          | 7      | sm(2)    | \-                                   | \-                                | 8                       | 33                   | \-                         | \-                      | 55.59           | 124           | 210             | 53              |
| 21          | 7      | inc(3)   | 13                                   | 71                                | 19                      | 104                  | 9                          | 49                      | 5.37            | 124           | 493             | 87              |
| 21          | 7      | sm(3)    | \-                                   | \-                                | 15                      | 82                   | \-                         | \-                      | 65.86           | 124           | 462             | 83              |
| 21          | 7      | inc(4)   | 30                                   | 199                               | 45                      | 285                  | 25                         | 162                     | 19.36           | 124           | 801             | 110             |
| 21          | 7      | sm(4)    | \-                                   | \-                                | 33                      | 227                  | \-                         | \-                      | 92.83           | 124           | 762             | 110             |
| 23          | 19     | inc(2)   | 8                                    | 36                                | 9                       | 42                   | 8                          | 36                      | 0.81            | 141           | 304             | 73              |
| 23          | 19     | sm(2)    | \-                                   | \-                                | 8                       | 34                   | \-                         | \-                      | 54.10           | 141           | 273             | 68              |
| 23          | 19     | inc(3)   | 18                                   | 95                                | 23                      | 119                  | 12                         | 59                      | 3.96            | 141           | 554             | 102             |
| 23          | 19     | sm(3)    | \-                                   | \-                                | 17                      | 94                   | \-                         | \-                      | 64.29           | 141           | 545             | 100             |
| 23          | 19     | inc(4)   | 43                                   | 278                               | 57                      | 355                  | 27                         | 166                     | 22.17           | 141           | 956             | 130             |
| 23          | 19     | sm(4)    | \-                                   | \-                                | 40                      | 272                  | \-                         | \-                      | 122.23          | 141           | 910             | 130             |
| 26          | 20     | inc(2)   | 5                                    | 27                                | 6                       | 33                   | 5                          | 27                      | 0.84            | 136           | 304             | 61              |
| 26          | 20     | sm(2)    | \-                                   | \-                                | 4                       | 23                   | \-                         | \-                      | 54.89           | 136           | 263             | 54              |
| 26          | 20     | inc(3)   | 14                                   | 87                                | 20                      | 121                  | 8                          | 50                      | 6.48            | 136           | 569             | 94              |
| 26          | 20     | sm(3)    | \-                                   | \-                                | 13                      | 84                   | \-                         | \-                      | 66.21           | 136           | 573             | 91              |
| 26          | 20     | inc(4)   | 38                                   | 273                               | 53                      | 357                  | 30                         | 211                     | 34.64           | 136           | 1003            | 125             |
| 26          | 20     | sm(4)    | \-                                   | \-                                | 36                      | 268                  | \-                         | \-                      | 130.52          | 136           | 922             | 122             |
| 27          | 11     | inc(2)   | 7                                    | 36                                | 9                       | 41                   | 7                          | 36                      | 1.19            | 141           | 296             | 69              |
| 27          | 11     | sm(2)    | \-                                   | \-                                | 7                       | 31                   | \-                         | \-                      | 52.08           | 141           | 298             | 68              |
| 27          | 11     | inc(3)   | 19                                   | 106                               | 22                      | 118                  | 15                         | 83                      | 3.22            | 141           | 567             | 97              |
| 27          | 11     | sm(3)    | \-                                   | \-                                | 16                      | 94                   | \-                         | \-                      | 63.38           | 141           | 493             | 96              |
| 27          | 11     | inc(4)   | 51                                   | 366                               | 55                      | 368                  | 34                         | 221                     | 2.45            | 141           | 1016            | 130             |
| 27          | 11     | sm(4)    | \-                                   | \-                                | 39                      | 280                  | \-                         | \-                      | 130.03          | 141           | 961             | 123             |
| 28          | 21     | inc(2)   | 7                                    | 36                                | 8                       | 42                   | 7                          | 36                      | 0.75            | 155           | 336             | 71              |
| 28          | 21     | sm(2)    | \-                                   | \-                                | 6                       | 30                   | \-                         | \-                      | 55.76           | 155           | 288             | 67              |
| 28          | 21     | inc(3)   | 19                                   | 116                               | 24                      | 133                  | 13                         | 73                      | 5.06            | 155           | 635             | 109             |
| 28          | 21     | sm(3)    | \-                                   | \-                                | 18                      | 105                  | \-                         | \-                      | 64.75           | 155           | 589             | 105             |
| 28          | 21     | inc(4)   | 51                                   | 338                               | 69                      | 444                  | 39                         | 252                     | 18.69           | 155           | 1232            | 137             |
| 28          | 21     | sm(4)    | \-                                   | \-                                | 49                      | 334                  | \-                         | \-                      | 125.29          | 155           | 1012            | 133             |
| 30          | 22     | inc(2)   | 7                                    | 32                                | 8                       | 38                   | 7                          | 32                      | 0.89            | 140           | 262             | 54              |
| 30          | 22     | sm(2)    | \-                                   | \-                                | 6                       | 28                   | \-                         | \-                      | 55.45           | 140           | 271             | 56              |
| 30          | 22     | inc(3)   | 17                                   | 94                                | 22                      | 116                  | 16                         | 86                      | 4.67            | 140           | 564             | 94              |
| 30          | 22     | sm(3)    | \-                                   | \-                                | 15                      | 91                   | \-                         | \-                      | 67.50           | 140           | 562             | 93              |
| 30          | 22     | inc(4)   | 43                                   | 284                               | 61                      | 418                  | 32                         | 203                     | 23.83           | 140           | 1097            | 127             |
| 30          | 22     | sm(4)    | \-                                   | \-                                | 38                      | 277                  | \-                         | \-                      | 125.71          | 140           | 950             | 125             |
| 31          | 23     | inc(2)   | 9                                    | 41                                | 10                      | 47                   | 9                          | 41                      | 0.77            | 158           | 317             | 69              |
| 31          | 23     | sm(2)    | \-                                   | \-                                | 8                       | 35                   | \-                         | \-                      | 58.58           | 158           | 271             | 64              |
| 31          | 23     | inc(3)   | 22                                   | 124                               | 29                      | 159                  | 16                         | 80                      | 5.78            | 158           | 598             | 106             |
| 31          | 23     | sm(3)    | \-                                   | \-                                | 20                      | 112                  | \-                         | \-                      | 67.77           | 158           | 606             | 104             |
| 31          | 23     | inc(4)   | 55                                   | 364                               | 80                      | 581                  | 34                         | 206                     | 23.57           | 158           | 1171            | 139             |
| 31          | 23     | sm(4)    | \-                                   | \-                                | 51                      | 343                  | \-                         | \-                      | 125.08          | 158           | 983             | 135             |
| 33          | 14     | inc(2)   | 5                                    | 26                                | 7                       | 31                   | 5                          | 26                      | 1.27            | 120           | 203             | 47              |
| 33          | 14     | sm(2)    | \-                                   | \-                                | 6                       | 26                   | \-                         | \-                      | 63.33           | 120           | 241             | 54              |
| 33          | 14     | inc(3)   | 14                                   | 82                                | 17                      | 88                   | 13                         | 75                      | 2.07            | 120           | 412             | 81              |
| 33          | 14     | sm(3)    | \-                                   | \-                                | 13                      | 75                   | \-                         | \-                      | 63.53           | 120           | 444             | 80              |
| 33          | 14     | inc(4)   | 39                                   | 260                               | 42                      | 275                  | 28                         | 185                     | 2.80            | 120           | 824             | 111             |
| 33          | 14     | sm(4)    | \-                                   | \-                                | 31                      | 220                  | \-                         | \-                      | 123.45          | 120           | 784             | 106             |
| 34          | 16     | inc(2)   | 5                                    | 26                                | 6                       | 30                   | 5                          | 26                      | 0.82            | 119           | 207             | 46              |
| 34          | 16     | sm(2)    | \-                                   | \-                                | 5                       | 25                   | \-                         | \-                      | 57.14           | 119           | 179             | 42              |
| 34          | 16     | inc(3)   | 14                                   | 82                                | 15                      | 85                   | 9                          | 51                      | 1.51            | 119           | 410             | 78              |
| 34          | 16     | sm(3)    | \-                                   | \-                                | 12                      | 72                   | \-                         | \-                      | 64.84           | 119           | 388             | 76              |
| 34          | 16     | inc(4)   | 38                                   | 261                               | 39                      | 267                  | 26                         | 175                     | 3.67            | 119           | 802             | 108             |
| 34          | 16     | sm(4)    | \-                                   | \-                                | 30                      | 215                  | \-                         | \-                      | 139.84          | 119           | 754             | 106             |
| 35          | 20     | inc(2)   | 5                                    | 26                                | 6                       | 33                   | 5                          | 26                      | 0.96            | 136           | 304             | 61              |
| 35          | 20     | sm(2)    | \-                                   | \-                                | 4                       | 23                   | \-                         | \-                      | 54.89           | 136           | 263             | 54              |
| 35          | 20     | inc(3)   | 14                                   | 80                                | 19                      | 108                  | 10                         | 56                      | 4.96            | 136           | 529             | 92              |
| 35          | 20     | sm(3)    | \-                                   | \-                                | 13                      | 84                   | \-                         | \-                      | 66.21           | 136           | 573             | 91              |
| 35          | 20     | inc(4)   | 38                                   | 261                               | 62                      | 453                  | 23                         | 155                     | 27.16           | 136           | 1097            | 123             |
| 35          | 20     | sm(4)    | \-                                   | \-                                | 36                      | 268                  | \-                         | \-                      | 130.52          | 136           | 922             | 122             |
| 36          | 15     | inc(2)   | 7                                    | 35                                | 9                       | 40                   | 7                          | 35                      | 0.98            | 139           | 275             | 61              |
| 36          | 15     | sm(2)    | \-                                   | \-                                | 7                       | 30                   | \-                         | \-                      | 54.21           | 139           | 266             | 62              |
| 36          | 15     | inc(3)   | 19                                   | 102                               | 22                      | 116                  | 15                         | 80                      | 2.26            | 139           | 598             | 98              |
| 36          | 15     | sm(3)    | \-                                   | \-                                | 16                      | 90                   | \-                         | \-                      | 65.04           | 139           | 595             | 101             |
| 36          | 15     | inc(4)   | 52                                   | 334                               | 55                      | 356                  | 28                         | 181                     | 2.61            | 139           | 924             | 119             |
| 36          | 15     | sm(4)    | \-                                   | \-                                | 39                      | 268                  | \-                         | \-                      | 106.27          | 139           | 890             | 115             |
| 39          | 15     | inc(2)   | 7                                    | 31                                | 9                       | 40                   | 7                          | 31                      | 1.20            | 139           | 275             | 61              |
| 39          | 15     | sm(2)    | \-                                   | \-                                | 7                       | 30                   | \-                         | \-                      | 54.21           | 139           | 266             | 62              |
| 39          | 15     | inc(3)   | 17                                   | 91                                | 24                      | 131                  | 17                         | 91                      | 5.54            | 139           | 553             | 95              |
| 39          | 15     | sm(3)    | \-                                   | \-                                | 16                      | 90                   | \-                         | \-                      | 65.04           | 139           | 595             | 101             |
| 39          | 15     | inc(4)   | 42                                   | 267                               | 63                      | 427                  | 26                         | 162                     | 25.72           | 139           | 1000            | 123             |
| 39          | 15     | sm(4)    | \-                                   | \-                                | 39                      | 268                  | \-                         | \-                      | 106.27          | 139           | 890             | 115             |
| 40          | 18     | inc(2)   | 7                                    | 31                                | 8                       | 35                   | 7                          | 31                      | 1.00            | 123           | 227             | 54              |
| 40          | 18     | sm(2)    | \-                                   | \-                                | 7                       | 30                   | \-                         | \-                      | 55.34           | 123           | 226             | 54              |
| 40          | 18     | inc(3)   | 17                                   | 88                                | 18                      | 97                   | 15                         | 78                      | 2.28            | 123           | 503             | 86              |
| 40          | 18     | sm(3)    | \-                                   | \-                                | 14                      | 79                   | \-                         | \-                      | 68.29           | 123           | 466             | 82              |
| 40          | 18     | inc(4)   | 42                                   | 275                               | 43                      | 274                  | 32                         | 201                     | 2.38            | 123           | 802             | 108             |
| 40          | 18     | sm(4)    | \-                                   | \-                                | 32                      | 224                  | \-                         | \-                      | 111.23          | 123           | 755             | 108             |
| 45          | 18     | inc(2)   | 5                                    | 28                                | 7                       | 33                   | 5                          | 28                      | 1.23            | 123           | 225             | 54              |
| 45          | 18     | sm(2)    | \-                                   | \-                                | 7                       | 30                   | \-                         | \-                      | 55.34           | 123           | 226             | 54              |
| 45          | 18     | inc(3)   | 14                                   | 87                                | 17                      | 95                   | 10                         | 60                      | 1.90            | 123           | 501             | 86              |
| 45          | 18     | sm(3)    | \-                                   | \-                                | 14                      | 79                   | \-                         | \-                      | 68.29           | 123           | 466             | 82              |
| 45          | 18     | inc(4)   | 38                                   | 260                               | 42                      | 268                  | 30                         | 200                     | 2.40            | 123           | 800             | 110             |
| 45          | 18     | sm(4)    | \-                                   | \-                                | 32                      | 224                  | \-                         | \-                      | 111.23          | 123           | 755             | 108             |
| 47          | 19     | inc(2)   | 7                                    | 33                                | 9                       | 42                   | 7                          | 33                      | 1.13            | 141           | 304             | 73              |
| 47          | 19     | sm(2)    | \-                                   | \-                                | 8                       | 34                   | \-                         | \-                      | 54.10           | 141           | 273             | 68              |
| 47          | 19     | inc(3)   | 17                                   | 90                                | 23                      | 130                  | 13                         | 68                      | 6.32            | 141           | 616             | 103             |
| 47          | 19     | sm(3)    | \-                                   | \-                                | 17                      | 94                   | \-                         | \-                      | 64.29           | 141           | 545             | 100             |
| 47          | 19     | inc(4)   | 42                                   | 269                               | 60                      | 381                  | 32                         | 202                     | 23.87           | 141           | 1007            | 131             |
| 47          | 19     | sm(4)    | \-                                   | \-                                | 40                      | 272                  | \-                         | \-                      | 122.23          | 141           | 910             | 130             |
| 48          | 21     | inc(2)   | 6                                    | 33                                | 8                       | 42                   | 6                          | 33                      | 1.49            | 155           | 336             | 71              |
| 48          | 21     | sm(2)    | \-                                   | \-                                | 6                       | 30                   | \-                         | \-                      | 55.76           | 155           | 288             | 67              |
| 48          | 21     | inc(3)   | 18                                   | 103                               | 26                      | 157                  | 11                         | 64                      | 6.24            | 155           | 705             | 108             |
| 48          | 21     | sm(3)    | \-                                   | \-                                | 18                      | 105                  | \-                         | \-                      | 64.75           | 155           | 589             | 105             |
| 48          | 21     | inc(4)   | 50                                   | 341                               | 65                      | 423                  | 34                         | 226                     | 19.87           | 155           | 1141            | 138             |
| 48          | 21     | sm(4)    | \-                                   | \-                                | 49                      | 334                  | \-                         | \-                      | 125.29          | 155           | 1012            | 133             |
| 49          | 22     | inc(2)   | 6                                    | 33                                | 8                       | 38                   | 6                          | 33                      | 1.45            | 140           | 262             | 54              |
| 49          | 22     | sm(2)    | \-                                   | \-                                | 6                       | 28                   | \-                         | \-                      | 55.45           | 140           | 271             | 56              |
| 49          | 22     | inc(3)   | 18                                   | 109                               | 21                      | 121                  | 12                         | 69                      | 1.96            | 140           | 625             | 98              |
| 49          | 22     | sm(3)    | \-                                   | \-                                | 15                      | 91                   | \-                         | \-                      | 67.50           | 140           | 562             | 93              |
| 49          | 22     | inc(4)   | 51                                   | 347                               | 54                      | 347                  | 32                         | 211                     | 3.99            | 140           | 990             | 126             |
| 49          | 22     | sm(4)    | \-                                   | \-                                | 38                      | 277                  | \-                         | \-                      | 125.71          | 140           | 950             | 125             |
| 51          | 23     | inc(2)   | 8                                    | 38                                | 10                      | 47                   | 8                          | 38                      | 1.36            | 158           | 317             | 69              |
| 51          | 23     | sm(2)    | \-                                   | \-                                | 8                       | 35                   | \-                         | \-                      | 58.58           | 158           | 271             | 64              |
| 51          | 23     | inc(3)   | 21                                   | 111                               | 29                      | 165                  | 15                         | 76                      | 5.62            | 158           | 669             | 106             |
| 51          | 23     | sm(3)    | \-                                   | \-                                | 20                      | 112                  | \-                         | \-                      | 67.77           | 158           | 606             | 104             |
| 51          | 23     | inc(4)   | 54                                   | 355                               | 80                      | 581                  | 44                         | 289                     | 23.20           | 158           | 1176            | 142             |
| 51          | 23     | sm(4)    | \-                                   | \-                                | 51                      | 343                  | \-                         | \-                      | 125.08          | 158           | 983             | 135             |
