# Soda Vending Machine Software Product Line
Soda vending machine SPL has 6 features and a core feature. The core of the product line represents the common behavior which exists in all products that belong to bank account product line. The core behavior is modelled using core ESG (c-ESG). An optional behavior is modelled using a feature ESG (f-ESG). A featured ESG (FESG) is an extended ESG that is composed of a core ESG (c-ESG) and a set of feature ESGs (f-ESGs). A featured ESG is used in test sequence composition approach which composes the sequences of core and feature ESGs and generates a product's test sequences. The models of soda vending machine SPL are built from the users' perspective. The Event Sequence Graph events are selected from user events. 

## Feature Model
![Feature Model](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/SodaVendingMachine/SodaVendingMachinePL_ModelImages/SodaVendingMachinePL_featureModel.PNG)

This feature model has 2 mandatory and 1 optional features. The abstract feature _ServeBeverage_ groups _serveSoda_ and _serveTea_ features with OR relationship likewise the _Purchase_ feature which groups _payEUR_, _payUSD_ and _free_ features. The feature _cancel_ is the optional feature of this SPL. Furthermore, there is an implication corresponds to require relationship where _cancel_ feature requires _payEUR_ feature or _payUSD_ feature in a product configuration.

# Soda Vending Machine Product Line Features
## Core ESG (c-ESG)
 ![core](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/SodaVendingMachine/SodaVendingMachinePL_ModelImages/core.PNG) \
 The core ESG of the soda vending machine product line represents core features, which exist in all product configurations. For this product line the core feature includes the "prompt" and "select" events of the soda vending machine.\
 [Core ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/SodaVendingMachine/SodaVendingMachinePL_Models/core.zip)
 
 ## Serve Soda Feature ESG (f-ESG)
 ![serveSoda](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/SodaVendingMachine/SodaVendingMachinePL_ModelImages/serveSoda.PNG) \
 Serve Soda f-ESG represents the serving soda operation of the soda vending machine .\
 [Serve Soda Feature ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/SodaVendingMachine/SodaVendingMachinePL_Models/serveSoda.zip)
 
  ## Serve Tea Feature ESG (f-ESG)
 ![serveTea](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/SodaVendingMachine/SodaVendingMachinePL_ModelImages/serveTea.PNG) \
 Serve Tea f-ESG represents the serving tea operation of the soda vending machine .\
 [Serve Tea Feature ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/SodaVendingMachine/SodaVendingMachinePL_Models/serveTea.zip)
 
  ## Pay EUR Feature ESG (f-ESG)
 ![payEUR](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/SodaVendingMachine/SodaVendingMachinePL_ModelImages/payEUR.PNG) \
 Pay EUR f-ESG brings the soda vending machine users the ability to pay in EUR currency.\
 [Pay EUR Feature ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/SodaVendingMachine/SodaVendingMachinePL_Models/payEUR.zip)
 
  ## Pay USD Feature ESG (f-ESG)
 ![payUSD](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/SodaVendingMachine/SodaVendingMachinePL_ModelImages/payUSD.PNG) \
 Pay USD f-ESG brings the soda vending machine users the ability to pay in USD currency.\
 [Pay USD Feature ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/SodaVendingMachine/SodaVendingMachinePL_Models/payUSD.zip)
 
 ## Cancel Feature ESG (f-ESG)
 ![cancel](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/SodaVendingMachine/SodaVendingMachinePL_ModelImages/cancel.PNG) \
Cancel f-ESG represents cancelling the payment both in EUR and USD currency.\
 [Cancel Feature ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/SodaVendingMachine/SodaVendingMachinePL_Models/cancel.zip)
  
 ## Free Feature ESG (f-ESG)
 ![free](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/SodaVendingMachine/SodaVendingMachinePL_ModelImages/free.PNG) \
  Free feature helps soda vending machine users to be served soda or tea free.\
[Free Feature ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/SodaVendingMachine/SodaVendingMachinePL_Models/free.zip)
   
 # Soda Vending Machine Example Products
  Below, some example products of Soda Vending Machine SPL are shown.
    
## Full Product ESG
  ![productFull](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/SodaVendingMachine/SodaVendingMachinePL_ModelImages/SodaVendingMachinePLProduct_fullProduct.PNG) \
  Full Product includes all of the 6 features in Soda Vending Machine SPL.\
  [Basic Product ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/SodaVendingMachine/SodaVendingMachinePL_Models/SodaVendingMachinePLProduct_fullProduct.zip)

## EUR-Soda Product ESG
  ![productEURSoda](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/SodaVendingMachine/SodaVendingMachinePL_ModelImages/SodaVendingMachinePLProduct_EURSodaProduct.PNG) \
  EUR-Soda Product has the _payEUR_ and _serveSoda_ features. The users of this account can select the beverage soda and pay in EUR.\
  [EUR-Soda Product ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/SodaVendingMachine/SodaVendingMachinePL_Models/SodaVendingMachinePLProduct_EURSodaProduct.zip)
  
## EUR-Soda-Cancel Product ESG
  ![productEURSodaCancel](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/SodaVendingMachine/SodaVendingMachinePL_ModelImages/SodaVendingMachinePLProduct_EURSodaCancelProduct.PNG) \
  EUR-Soda-Cancel Product has the _cancel_ feature in addition to the _payEUR_ and _serveSoda_ features. The users of this account can select the beverage soda and pay in EUR and cancel the payment if they would like to.\
  [EUR-Soda-Cancel Product ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/SodaVendingMachine/SodaVendingMachinePL_Models/SodaVendingMachinePLProduct_EURSodaCancelProduct.zip)

## Free Product ESG
![productFree](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/SodaVendingMachine/SodaVendingMachinePL_ModelImages/SodaVendingMachinePLProduct_freeProduct.PNG) \
Freee Product has serves soda beverage to the users for free.\
[Free Product ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/SodaVendingMachine/SodaVendingMachinePL_Models/SodaVendingMachinePLProduct_freeProduct.zip)

[Click to download all ESG MXE Files](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/SodaVendingMachine/SodaVendingMachinePL_Models/SodaVendingMachinePL_Models.zip)

  

