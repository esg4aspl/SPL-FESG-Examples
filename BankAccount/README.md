# Bank Account Product Line
The models of bank account product line are built from the users' perspective. The Event Sequence graphs' events are selected from user events. Bank account product line has nine features and a core feature. The core of the product line represents the common behavior which exists in all products that belong to bank account product line. The core behavior is modelled using core ESG (c-ESG).An optional behavior is modelled using a feature ESG (f-ESG). A featured ESG (FESG) is an extended ESG that is composed of a core ESG (c-ESG) and a set of feature ESGs (f-ESGs). A featured ESG is used in test sequence composition approach which composes the sequences of core and feature ESGs and generates a product's test sequences.

Scenario ID	Existing Product ID	Existing Product	Product Under Consideration ID	Product Under Consideration
2	0	baseProduct	6	cancelWithdraw
3	0	baseProduct	24	credit
5	1	interest	4	cancelDeposit_interest
64	24	credit	25	credit_interest
19	6	cancelWithdraw	7	interest_cancelWithdraw
66	24	credit	30	credit_cancelWithdraw
4	1	interest	2	interest_interestEstimation
20	6	cancelWithdraw	9	cancelWithdraw_dailyLimit
68	25	credit_interest	28	cancelDeposit_credit_interest
41	12	cancelDeposit_cancelWithdraw	13	cancelDeposit_interest_cancelWithdraw
31	9	cancelWithdraw_dailyLimit	15	cancelDeposit_cancelWithdraw_dailyLimit
67	25	credit_interest	26	credit_interest_interestEstimation
43	12	cancelDeposit_cancelWithdraw	36	cancelDeposit_credit_cancelWithdraw
23	7	interest_cancelWithdraw	8	interest_cancelWithdraw_interestEstimation
78	30	credit_cancelWithdraw	33	credit_cancelWithdraw_dailyLimit
17	5	cancelDeposit_interest_interestEstimation	14	cancelDeposit_interest_cancelWithdraw_interestEstimation
50	15	cancelDeposit_cancelWithdraw_dailyLimit	21	cancelDeposit_cancelWithdraw_dailyLimit_overdraft
86	33	credit_cancelWithdraw_dailyLimit	39	cancelDeposit_credit_cancelWithdraw_dailyLimit
71	26	credit_interest_interestEstimation	32	credit_interest_cancelWithdraw_interestEstimation
85	33	credit_cancelWithdraw_dailyLimit	34	credit_interest_cancelWithdraw_dailyLimit
49	15	cancelDeposit_cancelWithdraw_dailyLimit	16	cancelDeposit_interest_cancelWithdraw_dailyLimit
36	10	interest_cancelWithdraw_dailyLimit	19	interest_cancelWithdraw_dailyLimit_overdraft
54	16	cancelDeposit_interest_cancelWithdraw_dailyLimit	40	cancelDeposit_credit_interest_cancelWithdraw_dailyLimit
62	21	cancelDeposit_cancelWithdraw_dailyLimit_overdraft	22	cancelDeposit_interest_cancelWithdraw_dailyLimit_overdraft
76	29	cancelDeposit_credit_interest_interestEstimation	38	cancelDeposit_credit_interest_cancelWithdraw_interestEstimation
52	16	cancelDeposit_interest_cancelWithdraw_dailyLimit	17	cancelDeposit_interest_cancelWithdraw_dailyLimit_interestEstimation
83	32	credit_interest_cancelWithdraw_interestEstimation	35	credit_interest_cancelWithdraw_dailyLimit_interestEstimation
39	11	interest_cancelWithdraw_dailyLimit_interestEstimation	20	interest_cancelWithdraw_dailyLimit_interestEstimation_overdraft
55	17	cancelDeposit_interest_cancelWithdraw_dailyLimit_interestEstimation	23	cancelDeposit_interest_cancelWithdraw_dailyLimit_interestEstimation_overdraft
89	35	credit_interest_cancelWithdraw_dailyLimit_interestEstimation	41	cancelDeposit_credit_interest_cancelWithdraw_dailyLimit_interestEstimation


## Feature Model

![Feature Model](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_ModelImages/BankAccountPL_featureModel.PNG)

This feature model has two mandatory and seven optional features. The feature interest estimation implies interest; daily limit implies withdraw and cancel withdraw and, overdraft implies cancel withdraw and daily limit. This means that a product configuration which has one of the implying features i.e. cancel withdraw, interest estimation etc. must have the corresponding implied feature. Different product configurations could be obtained by combining these features. 

## Product Matrix
![Product Matrix](https://github.com/dilekozturk93/BankAccountProductLine/blob/master/BankAccount_ModelImages/productMatrix.PNG)

The product matrix demonstrates the product configurations.

## Core ESG (c-ESG)
 ![core](https://github.com/dilekozturk93/BankAccountProductLine/blob/master/BankAccount_ModelImages/core.PNG) \
 The core ESG of the bank account product line represents core features, which exist in all product configurations. For this product line the core feature is  getting the current balance of the account.\
 [Core ESG MXE File](https://github.com/dilekozturk93/BankAccountProductLine/blob/master/BankAccountModels/core.zip)
 
 ## Deposit Feature ESG (f-ESG)
 ![deposit](https://github.com/dilekozturk93/BankAccountProductLine/blob/master/BankAccount_ModelImages/deposit.PNG) \
 Deposit f-ESG represents the deposit operation i.e. putting money to the account operation.\
 [Deposit Feature ESG MXE File](https://github.com/dilekozturk93/BankAccountProductLine/blob/master/BankAccountModels/deposit.zip)
 
 ## Cancel Deposit Feature ESG (f-ESG)
 ![cancelDeposit](https://github.com/dilekozturk93/BankAccountProductLine/blob/master/BankAccount_ModelImages/cancelDeposit.PNG) \
Cancel deposit f-ESG represents cancelling the deposit.\
 [Cancel Deposit Feature ESG MXE File](https://github.com/dilekozturk93/BankAccountProductLine/blob/master/BankAccountModels/cancelDeposit.zip)
 
 ## Withdraw Feature ESG (f-ESG)
 ![withdraw](https://github.com/dilekozturk93/BankAccountProductLine/blob/master/BankAccount_ModelImages/withdraw.PNG) \
 Withdraw f-ESG brings bank account users the ability to take money from the account.\
 [Withdraw Feature ESG MXE File](https://github.com/dilekozturk93/BankAccountProductLine/blob/master/BankAccountModels/withdraw.zip)
 
 ## Cancel Withdraw Feature ESG (f-ESG)
 ![cancelWithdraw](https://github.com/dilekozturk93/BankAccountProductLine/blob/master/BankAccount_ModelImages/cancelWithdraw.PNG) \
Cancel withdraw f-ESG represents cancelling the withdraw operation. This feature cannot exist in product configurations without withdraw feature.\
 [Cancel Withdraw Feature ESG MXE File](https://github.com/dilekozturk93/BankAccountProductLine/blob/master/BankAccountModels/cancelWithdraw.zip)
 
 ## Daily Limit Feature ESG (f-ESG)
 ![dailyLimit](https://github.com/dilekozturk93/BankAccountProductLine/blob/master/BankAccount_ModelImages/dailyLimit.PNG) \
  Daily limit feature helps bank account users to limit the amount of money that can be taken from the account in a day.\
[Daily Limit Feature ESG MXE File](https://github.com/dilekozturk93/BankAccountProductLine/blob/master/BankAccountModels/dailyLimit.zip)
  
  ## Overdraft Feature ESG (f-ESG)
  ![overdraft](https://github.com/dilekozturk93/BankAccountProductLine/blob/master/BankAccount_ModelImages/overdraft.PNG) \
  Overdraft feature helps bank account users to limit the amount of withdrawal money that excesses the account balance. This feature cannot exist in product configurations without daily limit feature.\
  [Overdraft Feature ESG MXE File] .\(https://github.com/dilekozturk93/BankAccountProductLine/blob/master/BankAccount_ModelImages/overdraft.png)
  
  ## Credit Feature ESG (f-ESG)
  ![credit](https://github.com/dilekozturk93/BankAccountProductLine/blob/master/BankAccount_ModelImages/credit.PNG) \
  Credit feature helps users to take extra money as a debt.\
  [Credit Feature ESG MXE File](https://github.com/dilekozturk93/BankAccountProductLine/blob/master/BankAccountModels/credit.zip)
   
  ## Interest Feature ESG (f-ESG) 
  ![interest](https://github.com/dilekozturk93/BankAccountProductLine/blob/master/BankAccount_ModelImages/interest.PNG) \
  Interest feature helps bank account users to request an interest rate.\
  [Interest Feature ESG MXE File](https://github.com/dilekozturk93/BankAccountProductLine/blob/master/BankAccountModels/interest.zip)
  
  ## Interest Estimation Feature ESG (f-ESG)
  ![interestEstimation](https://github.com/dilekozturk93/BankAccountProductLine/blob/master/BankAccount_ModelImages/interestEstimation.PNG) \
  Interest estimation feature helps bank account users to find out total inerest gain for certain days.\
  [Interest Estimation Feature ESG MXE File](https://github.com/dilekozturk93/BankAccountProductLine/blob/master/BankAccountModels/interestEstimation.zip)
  
  # Bank Account Products
## Base Product ESG
  ![productBase](https://github.com/dilekozturk93/BankAccountProductLine/blob/master/BankAccount_ModelImages/bankAccountProduct_baseProduct.PNG) \
  Base Product has the deposit and the withdraw mandatory features. The users of this account can deposit money and withdraw money, only.\
  [Base Product ESG MXE File](https://github.com/dilekozturk93/BankAccountProductLine/blob/master/BankAccountModels/bankAccountProduct_baseProduct.zip)

## Cancellable Product ESG
  ![productCancellable](https://github.com/dilekozturk93/BankAccountProductLine/blob/master/BankAccount_ModelImages/bankAccountProduct_cancellable.PNG) \
  Cancellable Product has the cancel deposit and the cancel withdraw features. The users of this account can deposit money, withdraw money and cancel these operations.\
  [Cancellable Product ESG MXE File](https://github.com/dilekozturk93/BankAccountProductLine/blob/master/BankAccountModels/bankAccountProduct_cancellable.zip)
  
## Credit Product ESG
![productCredit](https://github.com/dilekozturk93/BankAccountProductLine/blob/master/BankAccount_ModelImages/bankAccountProduct_credit.PNG) \
The users of this product can withdraw extra money from the account as a debt.\
[Credit Product ESG MXE File](https://github.com/dilekozturk93/BankAccountProductLine/blob/master/BankAccountModels/bankAccountProduct_credit.zip)

## Daily Limit Product ESG
![productDailyLimit](https://github.com/dilekozturk93/BankAccountProductLine/blob/master/BankAccount_ModelImages/bankAccountProduct_dailyLimit.PNG) \
Daily Limit Product has the daily limit, withdraw and cancel withdraw features.The users of this account can witdraw money up to a limit.\
[Daily Limit Product ESG MXE File](https://github.com/dilekozturk93/BankAccountProductLine/blob/master/BankAccountModels/bankAccountProduct_dailyLimit.zip)

## Overdraft Product ESG
![productOverdraft](https://github.com/dilekozturk93/BankAccountProductLine/blob/master/BankAccount_ModelImages/bankAccountProduct_overdraft.PNG) \
Overdraft Product has the overdraft, cancel withdraw and daily limit features.The users of this account can take extra money from the account without interest rate.\
[Overdraft Product ESG MXE File](https://github.com/dilekozturk93/BankAccountProductLine/blob/master/BankAccountModels/bankAccountProduct_overdraft.zip)

## Interest Product ESG
![productInterest](https://github.com/dilekozturk93/BankAccountProductLine/blob/master/BankAccount_ModelImages/bankAccountProduct_interest.PNG) \
Interest Product has interest and interest estimation features. The users of this product can learn the estimated interest for left days, confirm a specific interest rate. \
[Interest Product ESG MXE File](https://github.com/dilekozturk93/BankAccountProductLine/blob/master/BankAccountModels/bankAccountProduct_interest.zip)

[Click to download all ESG MXE Files](https://github.com/dilekozturk93/BankAccountProductLine/blob/master/BankAccountModels/BankAccountAllModels.zip)
