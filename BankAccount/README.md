# Bank Account Product Line
The models of bank account product line are built from the users' perspective. The Event Sequence graphs' events are selected from user events. Bank account product line has nine features and a core feature. The core of the product line represents the common behavior which exists in all products that belong to bank account product line. The core behavior is modelled using core ESG (c-ESG).An optional behavior is modelled using a feature ESG (f-ESG). A featured ESG (FESG) is an extended ESG that is composed of a core ESG (c-ESG) and a set of feature ESGs (f-ESGs). A featured ESG is used in test sequence composition approach which composes the sequences of core and feature ESGs and generates a product's test sequences.

## Feature Model
![Feature Model](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_ModelImages/BankAccountPL_featureModel.PNG)

This feature model has two mandatory and seven optional features. The feature _interest estimation_ implies _interest_; _daily limit_ implies _withdraw_ and _cancel withdraw_ and, _overdraft_ implies _cancel withdraw_ and _daily limit_. This means that a product configuration which has one of the implying features i.e. cancel withdraw, interest estimation etc. must have the corresponding implied feature. Different product configurations could be obtained by combining these features. 

## Full Product Matrix
![Full Product Matrix](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_ModelImages/BankAccountPL_fullProductMatrix.png)

The full product matrix demonstrates the product configurations of the Bank Account Product Line feature model. There are fourty two product configurations. In the table below, the product id and the belonging features are given. 

| Product ID | Features                                                                                              |
| ---------- | ----------------------------------------------------------------------------------------------------- |
| 0          | deposit, withdraw                                                                                     |
| 1          | deposit, withdraw, interest                                                                           |
| 3          | deposit, withdraw, cancelDeposit                                                                      |
| 6          | deposit, withdraw, cancelWithdraw                                                                     |
| 24         | deposit, withdraw, credit                                                                             |
| 2          | deposit, withdraw, interest, interestEstimation                                                       |
| 4          | deposit, withdraw, cancelDeposit, interest                                                            |
| 7          | deposit, withdraw, interest, cancelWithdraw                                                           |
| 9          | deposit, withdraw, cancelWithdraw, dailyLimit                                                         |
| 12         | deposit, withdraw, cancelDeposit, cancelWithdraw                                                      |
| 25         | deposit, withdraw, credit, interest                                                                   |
| 27         | deposit, withdraw, cancelDeposit, credit                                                              |
| 30         | deposit, withdraw, credit, cancelWithdraw                                                             |
| 5          | deposit, withdraw, cancelDeposit, interest, interestEstimation                                        |
| 8          | deposit, withdraw, interest, cancelWithdraw, interestEstimation                                       |
| 10         | deposit, withdraw, interest, cancelWithdraw, dailyLimit                                               |
| 13         | deposit, withdraw, cancelDeposit, interest, cancelWithdraw                                            |
| 15         | deposit, withdraw, cancelDeposit, cancelWithdraw, dailyLimit                                          |
| 18         | deposit, withdraw, cancelWithdraw, dailyLimit, overdraft                                              |
| 26         | deposit, withdraw, credit, interest, interestEstimation                                               |
| 28         | deposit, withdraw, cancelDeposit, credit, interest                                                    |
| 31         | deposit, withdraw, credit, interest, cancelWithdraw                                                   |
| 33         | deposit, withdraw, credit, cancelWithdraw, dailyLimit                                                 |
| 36         | deposit, withdraw, cancelDeposit, credit, cancelWithdraw                                              |
| 11         | deposit, withdraw, interest, cancelWithdraw, dailyLimit, interestEstimation                           |
| 14         | deposit, withdraw, cancelDeposit, interest, cancelWithdraw, interestEstimation                        |
| 16         | deposit, withdraw, cancelDeposit, interest, cancelWithdraw, dailyLimit                                |
| 19         | deposit, withdraw, interest, cancelWithdraw, dailyLimit, overdraft                                    |
| 21         | deposit, withdraw, cancelDeposit, cancelWithdraw, dailyLimit, overdraft                               |
| 29         | deposit, withdraw, cancelDeposit, credit, interest, interestEstimation                                |
| 32         | deposit, withdraw, credit, interest, cancelWithdraw, interestEstimation                               |
| 34         | deposit, withdraw, credit, interest, cancelWithdraw, dailyLimit                                       |
| 37         | deposit, withdraw, cancelDeposit, credit, interest, cancelWithdraw                                    |
| 39         | deposit, withdraw, cancelDeposit, credit, cancelWithdraw, dailyLimit                                  |
| 17         | deposit, withdraw, cancelDeposit, interest, cancelWithdraw, dailyLimit, interestEstimation            |
| 20         | deposit, withdraw, interest, cancelWithdraw, dailyLimit, interestEstimation, overdraft                |
| 22         | deposit, withdraw, cancelDeposit, interest, cancelWithdraw, dailyLimit, overdraft                     |
| 35         | deposit, withdraw, credit, interest, cancelWithdraw, dailyLimit, interestEstimation                   |
| 38         | deposit, withdraw, cancelDeposit, credit, interest, cancelWithdraw, interestEstimation                |
| 40         | deposit, withdraw, cancelDeposit, credit, interest, cancelWithdraw, dailyLimit                        |
| 23         | deposit, withdraw, cancelDeposit, interest, cancelWithdraw, dailyLimit, interestEstimation, overdraft |
| 41         | deposit, withdraw, cancelDeposit, credit, interest, cancelWithdraw, dailyLimit, interestEstimation    |

# Bank Account Product Line Features
## Core ESG (c-ESG)
 ![core](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_ModelImages/core.PNG) \
 The core ESG of the bank account product line represents core features, which exist in all product configurations. For this product line the core feature is  getting the current balance of the account.\
 [Core ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_Models/core.zip)
 
 ## Deposit Feature ESG (f-ESG)
 ![deposit](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_ModelImages/deposit.PNG) \
 Deposit f-ESG represents the deposit operation i.e. putting money to the account operation.\
 [Deposit Feature ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_Models/deposit.zip)
 
 ## Cancel Deposit Feature ESG (f-ESG)
 ![cancelDeposit](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_ModelImages/cancelDeposit.PNG) \
Cancel deposit f-ESG represents cancelling the deposit.\
 [Cancel Deposit Feature ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_Models/cancelDeposit.zip)
 
 ## Withdraw Feature ESG (f-ESG)
 ![withdraw](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_ModelImages/withdraw.PNG) \
 Withdraw f-ESG brings bank account users the ability to take money from the account.\
 [Withdraw Feature ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_Models/withdraw.zip)
 
 ## Cancel Withdraw Feature ESG (f-ESG)
 ![cancelWithdraw](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_ModelImages/cancelWithdraw.PNG) \
Cancel withdraw f-ESG represents cancelling the withdraw operation. This feature cannot exist in product configurations without withdraw feature.\
 [Cancel Withdraw Feature ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_Models/cancelWithdraw.zip)
 
 ## Daily Limit Feature ESG (f-ESG)
 ![dailyLimit](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_ModelImages/dailyLimit.PNG) \
  Daily limit feature helps bank account users to limit the amount of money that can be taken from the account in a day.\
[Daily Limit Feature ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_Models/dailyLimit.zip)
  
  ## Overdraft Feature ESG (f-ESG)
  ![overdraft](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_ModelImages/overdraft.PNG) \
  Overdraft feature helps bank account users to limit the amount of withdrawal money that excesses the account balance. This feature cannot exist in product configurations without daily limit feature.\
  [Overdraft Feature ESG MXE File] .\(https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_Models/overdraft.zip)
  
  ## Credit Feature ESG (f-ESG)
  ![credit](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_ModelImages/credit.PNG) \
  Credit feature helps users to take extra money as a debt.\
  [Credit Feature ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_Models/credit.zip)
   
  ## Interest Feature ESG (f-ESG) 
  ![interest](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_ModelImages/interest.PNG) \
  Interest feature helps bank account users to request an interest rate.\
  [Interest Feature ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_Models/interest.zip)
  
  ## Interest Estimation Feature ESG (f-ESG)
  ![interestEstimation](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_ModelImages/interestEstimation.PNG) \
  Interest estimation feature helps bank account users to find out total inerest gain for certain days.\
  [Interest Estimation Feature ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_Models/interestEstimation.zip)
  
 
 # Bank Account Line Example Products
  Below, some example products of Bank Account Product Line are shown in the below partial product matrix. Products in the partial product matrix correspond to some products in the full product matrix. The only difference is that the products in the partial product matrix are named and are given here as examples.
  
  ![Partial Product Matrix](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_ModelImages/BankAccountPL_partialProductMatrix.png)
  
## Basic Product ESG
  ![productBasic](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_ModelImages/BankAccountPLProduct_BasicProduct.PNG) \
  Basic Product has the deposit and the withdraw mandatory features. The users of this account can deposit money and withdraw money, only.\
  [Basic Product ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_Models/BankAccountPLProduct_BasicProduct.zip)

## Cancel Withdraw Product ESG
  ![productCancelWithdraw](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_ModelImages/BankAccountPLProduct_CancelWithdraw.PNG) \
  Cancel Withdraw Product has the cancel withdraw feature additional to the mandatory features. The users of this account can deposit money, withdraw money and cancel withdraw operation.\
  [Cancel Withdraw Product ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_Models/BankAccountPLProduct_CancelWithdraw.zip)
  
## Credit Product ESG
![productCredit](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_ModelImages/BankAccountPLProduct_Credit.PNG) \
The users of this product can withdraw extra money from the account as a debt.\
[Credit Product ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_Models/BankAccountPLProduct_Credit.zip)

## Daily Limit Product ESG
![productDailyLimit](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_ModelImages/BankAccountPLProduct_DailyLimit.PNG) \
Daily Limit Product has the daily limit and cancel withdraw features additional to the mandatory features.The users of this account can witdraw money up to a limit.\
[Daily Limit Product ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_Models/BankAccountPLProduct_DailyLimit.zip)

## Overdraft Product ESG
![productOverdraft](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_ModelImages/BankAccountPLProduct_Overdraft.PNG) \
Overdraft Product has the overdraft, cancel withdraw and daily limit features additional to the mandatory features.The users of this account can take extra money from the account without interest rate.\
[Overdraft Product ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_Models/BankAccountPLProduct_Overdraft.zip)

## Interest Product ESG
![productInterest](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_ModelImages/BankAccountPLProduct_Interest.PNG) \
Interest Product has interest feature additional to the mandatory features. The users of this product can . \
[Interest Product ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_Models/BankAccountPLProduct_Interest.zip)

[Click to download all ESG MXE Files](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_Models/BankAccountPL_Models.zip)

  # Bank Account Product Line Experiments and Results
The Bank Account Product Line has forty two(42) product configurations and ninty seven(97) one-increment testing scenarios in total. In our study, we select thirty of the testing scenarios randomly. Below the table of the selected scenarios is given. 

| Scenario ID | Product Under Consideration ID | Existing Product ID | Existing Product Features                                                                  | New Feature        |
| ----------- | ------------------------------ | ------------------- | ------------------------------------------------------------------------------------------ | ------------------ |
| 2           | 6                              | 0                   | deposit, withdraw                                                                          | cancelWithdraw     |
| 3           | 24                             | 0                   | deposit, withdraw                                                                          | credit             |
| 5           | 4                              | 1                   | deposit, withdraw, interest                                                                | cancelDeposit      |
| 64          | 25                             | 24                  | deposit, withdraw, credit                                                                  | interest           |
| 19          | 7                              | 6                   | deposit, withdraw, cancelWithdraw                                                          | interest           |
| 66          | 30                             | 24                  | deposit, withdraw, credit                                                                  | cancelWithdraw     |
| 4           | 2                              | 1                   | deposit, withdraw, interest                                                                | interestEstimation |
| 20          | 9                              | 6                   | deposit, withdraw, cancelWithdraw                                                          | dailyLimit         |
| 68          | 28                             | 25                  | deposit, withdraw, credit, interest                                                        | cancelDeposit      |
| 41          | 13                             | 12                  | deposit, withdraw, cancelDeposit, cancelWithdraw                                           | interest           |
| 31          | 15                             | 9                   | deposit, withdraw, cancelWithdraw, dailyLimit                                              | cancelDeposit      |
| 67          | 26                             | 25                  | deposit, withdraw, credit, interest                                                        | interestEstimation |
| 43          | 36                             | 12                  | deposit, withdraw, cancelDeposit, cancelWithdraw                                           | credit             |
| 23          | 8                              | 7                   | deposit, withdraw, interest, cancelWithdraw                                                | interestEstimation |
| 78          | 33                             | 30                  | deposit, withdraw, credit, cancelWithdraw                                                  | dailyLimit         |
| 17          | 14                             | 5                   | deposit, withdraw, cancelDeposit, interest, interestEstimation                             | cancelWithdraw     |
| 50          | 21                             | 15                  | deposit, withdraw, cancelDeposit, cancelWithdraw, dailyLimit                               | overdraft          |
| 86          | 39                             | 33                  | deposit, withdraw, credit, cancelWithdraw, dailyLimit                                      | cancelDeposit      |
| 71          | 32                             | 26                  | deposit, withdraw, credit, interest, interestEstimation                                    | cancelWithdraw     |
| 85          | 34                             | 33                  | deposit, withdraw, credit, cancelWithdraw, dailyLimit                                      | interest           |
| 49          | 16                             | 15                  | deposit, withdraw, cancelDeposit, cancelWithdraw, dailyLimit                               | interest           |
| 36          | 19                             | 10                  | deposit, withdraw, interest, cancelWithdraw, dailyLimit                                    | overdraft          |
| 54          | 40                             | 16                  | deposit, withdraw, cancelDeposit, interest, cancelWithdraw, dailyLimit                     | credit             |
| 62          | 22                             | 21                  | deposit, withdraw, cancelDeposit, cancelWithdraw, dailyLimit, overdraft                    | interest           |
| 76          | 38                             | 29                  | deposit, withdraw, cancelDeposit, credit, interest, interestEstimation                     | cancelWithdraw     |
| 52          | 17                             | 16                  | deposit, withdraw, cancelDeposit, interest, cancelWithdraw, dailyLimit                     | interestEstimation |
| 83          | 35                             | 32                  | deposit, withdraw, credit, interest, cancelWithdraw, interestEstimation                    | dailyLimit         |
| 39          | 20                             | 11                  | deposit, withdraw, interest, cancelWithdraw, dailyLimit, interestEstimation                | overdraft          |
| 55          | 23                             | 17                  | deposit, withdraw, cancelDeposit, interest, cancelWithdraw, dailyLimit, interestEstimation | overdraft          |
| 89          | 41                             | 35                  | deposit, withdraw, credit, interest, cancelWithdraw, dailyLimit, interestEstimation        | cancelDeposit      |
Table: Testing Scenarios
