# Email Product Line 

Email product line has 5 features and a core feature. The core of the product line represents the common behavior which exists in all products that belong to email product line. The core behavior is modelled using core ESG (c-ESG). An optional behavior is modelled using a feature ESG (f-ESG). A featured ESG (FESG) is an extended ESG that is composed of a core ESG (c-ESG) and a set of feature ESGs (f-ESGs). A featured ESG is used in test sequence composition approach which composes the sequences of core and feature ESGs and generates a product's test sequences. The models of email product line are built from the users' perspective. The Event Sequence Graph events are selected from user events. 

## Feature Model

![Feature Model](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailPL_ModelImages/EmailPL_FeatureModel.PNG)\
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

 [Click for the PDF version of the table](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/Products.pdf)

# Email Product Line Features
## Core ESG (c-ESG)
 ![core](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailPL_ModelImages/core.PNG)\
 The core ESG of the Email product line represents core features, which exist in all product configurations. For this product line the core feature is composing a new email, sending an email and receiving an email. Note that, the product that has the ID 0, has only core feature since the core feature itself, is capable of generating test sequences.\
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
