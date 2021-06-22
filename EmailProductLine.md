# Email Product Line 

Email product line has five features and a core feature. 

Remember that the core of the product line represents the common behavior which exists in all products that belong to Email Product Line. The core behavior is modelled using core ESG (c-ESG).An optional behavior is modelled using a feature ESG (f-ESG). 

## Feature Model

![Feature Model](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailPL_ModelImages/EmailPL_featureModel.PNG)\
This feature model has five optional features. The feature encrypt implies keys. This means that a product configuration which has the implying feature i.e. encrypt must have the feature keys. Different product configurations could be obtained by combining these features. 

## Email Products
There are twenty four product configurations in Email Product Line. In the table below, the product id and the belonging features are given. Since, each possible product does not have a unique official name, we assign IDs to products to name them uniquely.

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

## Core ESG (c-ESG)
 ![core](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailPL_ModelImages/core.PNG)\
 The core ESG of the elevator product line represents core features, which exist in all product configurations. For this product line the core features are composing a new eamil, sending an email and receiving an email. Note that, the product that has the ID 0, has only core feature. \
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

# Email Product Line Experiments and Results
The Email Product Line has twenty four product configurations and fifty two one-increment testing scenarios in total. In our study, we select thirty of the testing scenarios randomly. Below, the table of the selected testing scenarios is given.

## Testing Scenarios
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
