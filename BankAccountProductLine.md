# Bank Account Product Line

The models of bank account product line are built from the users' perspective. The Event Sequence graphs' events are selected from user events. Bank account product line has nine features and a core feature. 

Remember that the core of the product line represents the common behavior which exists in all products that belong to Bank Account Product Line. The core behavior is modelled using core ESG (c-ESG).An optional behavior is modelled using a feature ESG (f-ESG).

## Feature Model

![Feature Model](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountModelImages/BankAccount_FeatureModel.png)

This feature model has nine optional features. The feature cancel withdraw implies withdraw; interest estimation implies interest and overdraft implies daily limit. This means that a product configuration which has one of the implying features i.e. cancel withdraw, interest estimation, overdraft must have the corresponding implied feature. Different product configurations could be obtained by combining these features. 

## Product Table
![Product Table](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountModelImages/BankAccount_ConfigurationMap.png)

## Core ESG (c-ESG)
 ![core](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountModelImages/core.png)
 The core ESG of the bank account product line represents core features, which exist in all product configurations. For this product line the core features are putting money into an account and getting the current balance of the account.\
 [Core ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountModels/core.mxe)
 
 ## Cancel Deposit Feature ESG (f-ESG)
 ![cancelDeposit](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountModelImages/cancelDeposit.png)
Cancel deposit f-ESG represents cancelling the deposit i.e. putting money to the account operation.\
 [Cancel Deposit Feature ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountModels/cancelDeposit.mxe)
 
 ## Withdraw Feature ESG (f-ESG)
 ![withdraw](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountModelImages/withdraw.png)
 Withdraw f-ESG brings bank account users the ability to take money from the account.\
 [Withdraw Feature ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountModels/withdraw.mxe)
 
 ## Cancel Withdraw Feature ESG (f-ESG)
 ![cancelWithdraw](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountModelImages/cancelWithdraw.png)
Cancel withdraw f-ESG represents cancelling the withdraw operation. This feature cannot exist in product configurations without withdraw feature.\
 [Cancel Withdraw Feature ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountModels/cancelWithdraw.mxe)
 
 ## Daily Limit Feature ESG (f-ESG)
 ![dailyLimit](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountModelImages/dailyLimit.png)
  Daily limit feature helps bank account users to limit the amount of money that can be taken from the account in a day.\
  [Daily Limit Feature ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountModels/dailyLimit.mxe)
  
  ## Overdraft Feature ESG (f-ESG)
  ![overdraft](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountModelImages/overdraft.png)
  Overdraft feature helps bank account users to limit the amount of withdrawal money that excesses the account balance. This feature cannot exist in product configurations without daily limit feature.\
  [Overdraft Feature ESG MXE File] (https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountModels/overdraft.mxe)
   
  ## Interest Feature ESG (f-ESG)
  ![interest](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountModelImages/interest.png)
  Interest feature helps bank account users to request an interest rate.\
  [Interest Feature ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountModels/interest.mxe)
  
  ## Interest Estimation Feature ESG (f-ESG)
  ![interestEstimation](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountModelImages/interestEstimation.png)
  Interest estimation feature helps bank account users to find out total inerest gain for certain days.\
  [Interest Estimation Feature ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountModels/interestEstimation.mxe)
  
  ## Lock Feature ESG (f-ESG)
  ![lock](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountModelImages/lock.png)
  Lock feature helps users to lock and unlock the account from deposit and withdraw operations.\
  [Lock Feature ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountModels/lock.mxe)
  
  # Bank Account Products
  
  ## Cancel Deposit Product ESG
  ![productCancelDeposit](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountModelImages/bankAccountProduct_cancelDeposit.png)
  Cancel Deposit Product has the cancel deposit feature only. The users of this account can deposit money and cancel the deposit operation.\
  [Cancel Deposit Product ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountModels/bankAccountProduct_cancelDeposit.mxe)
  
## Withdraw Product ESG
![productWithdraw](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountModelImages/bankAccountProduct_withdraw.png)
The users of this product can withdraw money from the account.\
[Withdraw Product ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountModels/bankAccountProduct_withdraw.mxe)

## Cancel Deposit Withdraw Product ESG
![productCancelDepositWithdraw](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountModelImages/bankAccountProduct_cancelDepositWithdraw.png)
Cacel Deposit Withdraw Product has the cancel deposit and withdraw features.The users of this account can deposit money, cancel the deposit operation and withdraw money from account.\
[Cancel Deposit Withdraw Product ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountModels/bankAccountProduct_cancelDepositWithdraw.mxe)

## Cancel Deposit Withdraw Cancel Withdraw Product ESG
![productCancelDepositWithdrawCancelWithdraw](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountModelImages/bankAccountProduct_cancelDepositWithdrawCancelWithdraw.png)
Cacel Deposit Withdraw Product has the cancel deposit and withdraw features.The users of this account can deposit money, cancel the deposit operation and withdraw money from account.\
[Cancel Deposit Withdraw Cancel Withdraw Product ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountModels/bankAccountProduct_cancelDepositWithdrawCancelWithdraw.mxe)

## Lock Product ESG
![productLock](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountModelImages/bankAccountProduct_lock.png)
Lock Product has lock feature. The users of this product can lock and unlock the account. \
[Lock Product ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountModels/bankAccountProduct_lock.mxe)

## Lock Withdraw Product ESG
![productLockWithdraw](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountModelImages/bankAccountProduct_lockWithdraw.png)
Lock Product has lock feature. The users of this product can lock and unlock the account.\
[Lock Withdraw Product ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountModels/bankAccountProduct_lockWithdraw.mxe)

## Full Product ESG
![fullProduct](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountModelImages/bankAccountProduct_fullProduct.png)
Full Product has all nine features in the bank account product line.\
[Full Product ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountModels/bankAccountProduct_fullProduct.mxe)

[Click to download all ESG MXE Files](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountModels/BankAccountAllModels.zip)
