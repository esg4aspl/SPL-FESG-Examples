# Email Product Line 

Email product line has six features and a core feature. 

Remember that the core of the product line represents the common behavior which exists in all products that belong to Email Product Line. The core behavior is modelled using core ESG (c-ESG).An optional behavior is modelled using a feature ESG (f-ESG). 

## Feature Model

![Feature Model](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModelImages/EmailPL_FeatureModel.png)\
This feature model has five optional features. The feature encrypt implies keys. This means that a product configuration which has the implying feature i.e. encrypt must have the feature keys. Different product configurations could be obtained by combining these features. 

## Product Table
![Product Table](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModelImages/Email_ConfigurationMap.png)

## Core ESG (c-ESG)
 ![core](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModelImages/core.png)
 The core ESG of the elevator product line represents core features, which exist in all product configurations. For this product line the core features are composing a new eamil, sending an email and receiving an email.\
 [Core ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModels/core.mxe)

## Addressbook Feature ESG (f-ESG)
![addressbook](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModelImages/addressbook.png)
Addressbook feature helps a user to create an addressbook for a contact who has more than one email address and to send an email to all of the contact's email addresses.\
[Addressbook Feature ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModels/addressbook.mxe)

## Autoresponder Feature ESG (f-ESG)
![autoresponder](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModelImages/autoresponder.png)
Autoresponder feature helps the user to compose a autoresponse email body and set the date interval of autoresponse.\
[Autoresponder Feature ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModels/autoresponder.mxe)

## Forward Feature ESG (f-ESG)
![forward](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModelImages/forward.png)
Forward activates the email account's forwarding email feature. \
[Forward Feature ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModels/forward.mxe)

## Keys Feature ESG (f-ESG)
![keys](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModelImages/keys.png)
Keys feature aids the user to get one of its contact's public key su that the user can encrypt the sending email.\
[Keys Feature ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModels/keys.mxe)

## Encrypt Feature ESG (f-ESG)
![encrypt](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModelImages/encrypt.png)
Encrypt feature helps the user to encrypt the sending email. This feature implies keys feature since the  receiver's public key must be known to encrypt an email.\
[Encrypt Feature ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModels/encrypt.mxe)

## Sign Feature ESG (f-ESG)
![sign](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModelImages/sign.png)
Sign feature adds sender's signature to the email.\
[Sign Feature ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModels/sign.mxe)

 # Email Products
 
 ## Addressbook Product ESG
![productAddressbook](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModelImages/emailProduct_addressbook.png)
Addressbook is the only feature this product has.\
[Addressbook Product ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModels/emailProduct_addressbook.mxe)

 ## Autoresponder Product ESG
![productAutoresponder](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModelImages/emailProduct_autoresponder.png)
This product has only the autoresponder feature.\
[Autoresponder Product ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModels/emailProduct_autoresponder.mxe)

 ## Forward Product ESG
![productForward](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModelImages/emailProduct_forward.png)
This product allows only forwarding emails.\
[Forward Product ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModels/emailProduct_forward.mxe)

 ## Encrypt Product ESG
![productEncrypt](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModelImages/emailProduct_encrypt.png)
The users of this product can encrypt the sending emails. This product has also keys feature but keys feature does not make sense on its own existence.\
[Encrypt Product ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModels/emailProduct_encrypt.mxe)

 ## Addressbook Autoresponder Product ESG
![productAddressbookAutoresponder](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModelImages/emailProduct_addressbookAutoresponder.png)
This product has addressbook and autoresponder features.\
[Addressbook Autoresponder Product ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModels/emailProduct_addressbookAutoresponder.mxe)

 ## Addressbook Autoresponder Forward Product ESG
![productAddressbookAutoresponderForward](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModelImages/emailProduct_addressbookAutoresponderForward.png)
This product has addressbook, autoresponder and forward features.\
[Addressbook Autoresponder Forward Product ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModels/emailProduct_addressbookAutoresponderForward.mxe)

 ## Addressbook Autoresponder Encrypt Product ESG
![productAddressbookAutoresponderEncrypt](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModelImages/emailProduct_addressbookAutoresponderEncrypt.png)
This product has addressbook, autoresponder and encrypt features.\
[Addressbook Autoresponder Encrypt Product ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModels/emailProduct_addressbookAutoresponderEncrypt.mxe)

 ## Addressbook Autoresponder Sign Product ESG
![productAddressbookAutoresponderSign](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModelImages/emailProduct_addressbookAutoresponderSign.png)
This product has addressbook, autoresponder and sign features.\
[Addressbook Autoresponder Sign Product ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModels/emailProduct_addressbookAutoresponderSign.mxe)

 ## Addressbook Autoresponder Encrypt Sign Product ESG
![productAddressbookAutoresponderEncryptSign](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModelImages/emailProduct_addressbookAutoresponderEncryptSign.png)
This product has addressbook, autoresponder, encrypt and sign features.\
[Addressbook Autoresponder Encrypt Sign Product ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModels/emailProduct_addressbookAutoresponderEncryptSign.mxe)

 ## Addressbook Encrypt Product ESG
![productAddressbookEncrypt](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModelImages/emailProduct_addressbookEncrypt.png)
This product has addressbook and encrypt features.\
[Addressbook Encrypt Product ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModels/emailProduct_addressbookEncrypt.mxe)

 ## Autoresponder Encrypt Product ESG
![productAutoresponderEncrypt](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModelImages/emailProduct_autoresponderEncrypt.png)
This product has autoresponder and encrypt features.\
[Autoresponder Encrypt Product ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModels/emailProduct_addressbookAutoresponderEncrypt.mxe)

 ## Autoresponder Forward Product ESG
![productAutoresponderForward](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModelImages/emailProduct_autoresponderForward.png)
This product has autoresponder and forward features.\
[Autoresponder Forward Product ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModels/emailProduct_autoresponderForward.mxe)

[Click to download all ESG MXE Files](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/Email/EmailModels/EmailAllModels.zip)
