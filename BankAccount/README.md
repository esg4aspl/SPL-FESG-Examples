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

## Testing Scenarios
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

## Data on Product Under Consideration (PUC)
| Product Under Consideration ID | k = 1 |  k = 2 | k = 3 | k = 4 |
| ------------------------------ | ----- | ------ | ----- | ----- |
| 6                              | 8     | 9      | 11    | 14    |
| 24                             | 10    | 10     | 10    | 12    |
| 4                              | 11    | 11     | 11    | 14    |
| 25                             | 13    | 12     | 10    | 12    |
| 7                              | 11    | 11     | 11    | 14    |
| 30                             | 11    | 11     | 11    | 14    |
| 2                              | 12    | 12     | 12    | 13    |
| 9                              | 10    | 13     | 17    | 23    |
| 28                             | 14    | 13     | 11    | 14    |
| 13                             | 12    | 12     | 12    | 16    |
| 15                             | 11    | 14     | 18    | 25    |
| 26                             | 15    | 14     | 12    | 13    |
| 36                             | 12    | 12     | 12    | 16    |
| 8                              | 13    | 13     | 13    | 15    |
| 33                             | 13    | 15     | 17    | 23    |
| 14                             | 14    | 14     | 14    | 17    |
| 21                             | 13    | 17     | 21    | 29    |
| 39                             | 14    | 16     | 18    | 25    |
| 32                             | 16    | 15     | 13    | 15    |
| 34                             | 16    | 17     | 17    | 23    |
| 16                             | 14    | 16     | 18    | 25    |
| 19                             | 15    | 18     | 20    | 27    |
| 40                             | 17    | 18     | 18    | 25    |
| 22                             | 16    | 19     | 21    | 29    |
| 38                             | 17    | 16     | 14    | 17    |
| 17                             | 16    | 18     | 20    | 26    |
| 35                             | 18    | 19     | 19    | 24    |
| 20                             | 17    | 20     | 22    | 28    |
| 23                             | 18    | 21     | 23    | 30    |
| 41                             | 19    | 20     | 20    | 26    |

## Data on Number of Faults
| PUC ID | m=2 | m=3 | m=4 | m=5 | Total Number of Seeded Faults |
| ------ | --- | --- | --- | --- | ----------------------------- |
| 6      | 17  | 20  | 25  | 30  | 18                            |
| 24     | 20  | 20  | 22  | 26  | 18                            |
| 2      | 24  | 24  | 25  | 27  | 20                            |
| 4      | 22  | 22  | 25  | 30  | 20                            |
| 14     | 28  | 28  | 31  | 35  | 24                            |
| 7      | 22  | 22  | 25  | 30  | 20                            |
| 9      | 23  | 30  | 40  | 53  | 29                            |
| 8      | 26  | 26  | 28  | 31  | 22                            |
| 15     | 25  | 32  | 43  | 57  | 31                            |
| 19     | 33  | 38  | 47  | 62  | 36                            |
| 20     | 37  | 42  | 50  | 63  | 38                            |
| 13     | 24  | 24  | 28  | 34  | 22                            |
| 36     | 24  | 24  | 28  | 34  | 22                            |
| 16     | 30  | 34  | 43  | 57  | 33                            |
| 21     | 30  | 38  | 50  | 66  | 37                            |
| 17     | 34  | 38  | 46  | 58  | 35                            |
| 40     | 35  | 36  | 43  | 57  | 34                            |
| 23     | 39  | 44  | 53  | 67  | 41                            |
| 22     | 35  | 40  | 50  | 66  | 38                            |
| 25     | 25  | 22  | 22  | 26  | 19                            |
| 30     | 22  | 22  | 25  | 30  | 20                            |
| 26     | 29  | 26  | 25  | 27  | 21                            |
| 28     | 27  | 24  | 25  | 30  | 21                            |
| 32     | 31  | 28  | 28  | 31  | 24                            |
| 38     | 33  | 30  | 31  | 35  | 26                            |
| 33     | 28  | 32  | 40  | 53  | 31                            |
| 35     | 37  | 38  | 43  | 54  | 34                            |
| 34     | 33  | 34  | 40  | 53  | 32                            |
| 39     | 30  | 34  | 43  | 57  | 33                            |
| 41     | 39  | 40  | 46  | 58  | 37                            |

## Data on Test Generation and Execution

| PUC ID | Test Set | Existing Product Number of Sequences | Existing Product Number of Events | PUC Number of Sequences | PUC Number of Events | Number of Common Sequences | Number of Common Events | Generation Time | Faults Seeded | Events Executed | Faults Revealed |
| ------ | -------- | ------------------------------------ | --------------------------------- | ----------------------- | -------------------- | -------------------------- | ----------------------- | --------------- | ------------- | --------------- | --------------- |
| 6      | inc(2)   | 3                                    | 15                                | 4                       | 17                   | 3                          | 15                      | 0.8             | 18            | 67              | 13              |
| sm(2)  | \-       | \-                                   | 4                                 | 17                      | \-                   | \-                         | 64.11                   | 67              | 13            |
| inc(3) | 5        | 32                                   | 7                                 | 45                      | 5                    | 32                         | 2.69                    | 151             | 18            |
| sm(3)  | \-       | \-                                   | 6                                 | 36                      | \-                   | \-                         | 66.81                   | 148             | 18            |
| inc(4) | 6        | 39                                   | 8                                 | 55                      | 6                    | 39                         | 6.47                    | 173             | 18            |
| sm(4)  | \-       | \-                                   | 7                                 | 47                      | \-                   | \-                         | 69.11                   | 205             | 18            |
| 24     | inc(2)   | 3                                    | 15                                | 5                       | 19                   | 3                          | 15                      | 1.45            | 18            | 56              | 13              |
| sm(2)  | \-       | \-                                   | 5                                 | 19                      | \-                   | \-                         | 63.01                   | 56              | 13            |
| inc(3) | 5        | 32                                   | 8                                 | 43                      | 5                    | 32                         | 2.86                    | 131             | 18            |
| sm(3)  | \-       | \-                                   | 6                                 | 36                      | \-                   | \-                         | 58.64                   | 164             | 18            |
| inc(4) | 6        | 39                                   | 8                                 | 43                      | 6                    | 39                         | 3.98                    | 131             | 18            |
| sm(4)  | \-       | \-                                   | 4                                 | 32                      | \-                   | \-                         | 57.8                    | 128             | 16            |
| 2      | inc(2)   | 5                                    | 19                                | 6                       | 23                   | 5                          | 19                      | 0.83            | 20            | 78              | 16              |
| sm(2)  | \-       | \-                                   | 6                                 | 23                      | \-                   | \-                         | 75.56                   | 78              | 16            |
| inc(3) | 8        | 39                                   | 9                                 | 43                      | 8                    | 39                         | 2.01                    | 159             | 20            |
| sm(3)  | \-       | \-                                   | 7                                 | 40                      | \-                   | \-                         | 67.29                   | 160             | 20            |
| inc(4) | 8        | 39                                   | 9                                 | 43                      | 8                    | 39                         | 4.07                    | 159             | 20            |
| sm(4)  | \-       | \-                                   | 5                                 | 36                      | \-                   | \-                         | 73.28                   | 156             | 20            |
| 4      | inc(2)   | 5                                    | 19                                | 6                       | 21                   | 5                          | 19                      | 0.99            | 20            | 68              | 13              |
| sm(2)  | \-       | \-                                   | 6                                 | 21                      | \-                   | \-                         | 52.38                   | 84              | 13            |
| inc(3) | 8        | 39                                   | 11                                | 54                      | 8                    | 39                         | 2.2                     | 149             | 19            |
| sm(3)  | \-       | \-                                   | 8                                 | 40                      | \-                   | \-                         | 63.49                   | 191             | 19            |
| inc(4) | 8        | 39                                   | 12                                | 64                      | 8                    | 39                         | 6.57                    | 169             | 20            |
| sm(4)  | \-       | \-                                   | 7                                 | 47                      | \-                   | \-                         | 61.36                   | 142             | 17            |
| 14     | inc(2)   | 6                                    | 23                                | 7                       | 25                   | 6                          | 23                      | 0.82            | 24            | 68              | 16              |
| sm(2)  | \-       | \-                                   | 8                                 | 27                      | \-                   | \-                         | 55.26                   | 128             | 20            |
| inc(3) | 10       | 49                                   | 12                                | 62                      | 10                   | 49                         | 2.61                    | 157             | 21            |
| sm(3)  | \-       | \-                                   | 11                                | 48                      | \-                   | \-                         | 68.64                   | 163             | 23            |
| inc(4) | 12       | 62                                   | 14                                | 78                      | 12                   | 62                         | 3.85                    | 199             | 24            |
| sm(4)  | \-       | \-                                   | 11                                | 66                      | \-                   | \-                         | 69.48                   | 175             | 24            |
| 7      | inc(2)   | 4                                    | 17                                | 6                       | 21                   | 4                          | 17                      | 1.2             | 20            | 75              | 14              |
| sm(2)  | \-       | \-                                   | 6                                 | 21                      | \-                   | \-                         | 56.06                   | 75              | 14            |
| inc(3) | 8        | 43                                   | 11                                | 54                      | 8                    | 43                         | 2.96                    | 161             | 20            |
| sm(3)  | \-       | \-                                   | 8                                 | 40                      | \-                   | \-                         | 61.87                   | 209             | 19            |
| inc(4) | 10       | 56                                   | 12                                | 60                      | 10                   | 56                         | 3.63                    | 175             | 20            |
| sm(4)  | \-       | \-                                   | 7                                 | 47                      | \-                   | \-                         | 66.43                   | 220             | 19            |
| 9      | inc(2)   | 4                                    | 17                                | 7                       | 28                   | 4                          | 17                      | 2.43            | 29            | 110             | 24              |
| sm(2)  | \-       | \-                                   | 7                                 | 28                      | \-                   | \-                         | 51.31                   | 118             | 24            |
| inc(3) | 8        | 43                                   | 14                                | 81                      | 8                    | 43                         | 7.46                    | 239             | 26            |
| sm(3)  | \-       | \-                                   | 9                                 | 50                      | \-                   | \-                         | 63.17                   | 244             | 28            |
| inc(4) | 10       | 56                                   | 20                                | 126                     | 10                   | 56                         | 14.57                   | 310             | 29            |
| sm(4)  | \-       | \-                                   | 13                                | 78                      | \-                   | \-                         | 70.92                   | 230             | 29            |
| 8      | inc(2)   | 6                                    | 21                                | 7                       | 25                   | 6                          | 21                      | 0.94            | 22            | 77              | 16              |
| sm(2)  | \-       | \-                                   | 7                                 | 25                      | \-                   | \-                         | 71.48                   | 83              | 17            |
| inc(3) | 11       | 54                                   | 11                                | 51                      | 10                   | 47                         | 2.02                    | 141             | 20            |
| sm(3)  | \-       | \-                                   | 9                                 | 44                      | \-                   | \-                         | 55.89                   | 164             | 19            |
| inc(4) | 11       | 53                                   | 12                                | 57                      | 11                   | 53                         | 3.23                    | 159             | 22            |
| sm(4)  | \-       | \-                                   | 8                                 | 51                      | \-                   | \-                         | 59.05                   | 147             | 21            |
| 15     | inc(2)   | 7                                    | 28                                | 8                       | 30                   | 7                          | 28                      | 0.82            | 31            | 128             | 23              |
| sm(2)  | \-       | \-                                   | 8                                 | 30                      | \-                   | \-                         | 52.44                   | 147             | 21            |
| inc(3) | 13       | 62                                   | 16                                | 77                      | 13                   | 62                         | 2.45                    | 240             | 29            |
| sm(3)  | \-       | \-                                   | 11                                | 54                      | \-                   | \-                         | 63.85                   | 255             | 28            |
| inc(4) | 18       | 91                                   | 21                                | 109                     | 18                   | 91                         | 3.67                    | 286             | 30            |
| sm(4)  | \-       | \-                                   | 16                                | 93                      | \-                   | \-                         | 69.81                   | 247             | 29            |
| 19     | inc(2)   | 9                                    | 32                                | 12                      | 43                   | 9                          | 32                      | 1.7             | 36            | 115             | 23              |
| sm(2)  | \-       | \-                                   | 12                                | 43                      | \-                   | \-                         | 58.12                   | 131             | 23            |
| inc(3) | 15       | 66                                   | 20                                | 90                      | 15                   | 66                         | 5.76                    | 204             | 30            |
| sm(3)  | \-       | \-                                   | 14                                | 66                      | \-                   | \-                         | 61.61                   | 209             | 27            |
| inc(4) | 20       | 95                                   | 27                                | 127                     | 18                   | 78                         | 17.76                   | 283             | 34            |
| sm(4)  | \-       | \-                                   | 16                                | 93                      | \-                   | \-                         | 65.83                   | 259             | 28            |
| 20     | inc(2)   | 9                                    | 34                                | 12                      | 45                   | 9                          | 34                      | 1.44            | 38            | 155             | 30              |
| sm(2)  | \-       | \-                                   | 13                                | 47                      | \-                   | \-                         | 63.00                   | 157             | 30            |
| inc(3) | 16       | 75                                   | 20                                | 92                      | 16                   | 75                         | 6.38                    | 258             | 36            |
| sm(3)  | \-       | \-                                   | 15                                | 70                      | \-                   | \-                         | 72.99                   | 237             | 34            |
| inc(4) | 21       | 104                                  | 28                                | 133                     | 19                   | 87                         | 16.87                   | 305             | 37            |
| sm(4)  | \-       | \-                                   | 17                                | 97                      | \-                   | \-                         | 71.67                   | 234             | 35            |
| 13     | inc(2)   | 5                                    | 19                                | 7                       | 23                   | 5                          | 19                      | 1.32            | 22            | 71              | 14              |
| sm(2)  | \-       | \-                                   | 7                                 | 23                      | \-                   | \-                         | 55.55                   | 81              | 15            |
| inc(3) | 10       | 51                                   | 13                                | 62                      | 10                   | 51                         | 2.75                    | 170             | 20            |
| sm(3)  | \-       | \-                                   | 10                                | 44                      | \-                   | \-                         | 63.43                   | 164             | 20            |
| inc(4) | 13       | 70                                   | 15                                | 74                      | 13                   | 70                         | 4.15                    | 198             | 22            |
| sm(4)  | \-       | \-                                   | 10                                | 62                      | \-                   | \-                         | 57.68                   | 196             | 21            |
| 36     | inc(2)   | 5                                    | 19                                | 7                       | 23                   | 5                          | 19                      | 1.21            | 22            | 71              | 14              |
| sm(2)  | \-       | \-                                   | 7                                 | 23                      | \-                   | \-                         | 55.55                   | 81              | 15            |
| inc(3) | 10       | 51                                   | 13                                | 62                      | 10                   | 51                         | 2.55                    | 170             | 20            |
| sm(3)  | \-       | \-                                   | 10                                | 44                      | \-                   | \-                         | 63.43                   | 164             | 20            |
| inc(4) | 13       | 70                                   | 15                                | 74                      | 13                   | 70                         | 3.92                    | 198             | 22            |
| sm(4)  | \-       | \-                                   | 10                                | 62                      | \-                   | \-                         | 57.68                   | 188             | 21            |
| 16     | inc(2)   | 8                                    | 30                                | 10                      | 34                   | 8                          | 30                      | 1.14            | 33            | 124             | 23              |
| sm(2)  | \-       | \-                                   | 10                                | 34                      | \-                   | \-                         | 55.94                   | 128             | 22            |
| inc(3) | 16       | 77                                   | 18                                | 81                      | 16                   | 77                         | 2.71                    | 232             | 31            |
| sm(3)  | \-       | \-                                   | 13                                | 58                      | \-                   | \-                         | 62.88                   | 243             | 30            |
| inc(4) | 22       | 112                                  | 24                                | 116                     | 22                   | 112                        | 4.25                    | 285             | 32            |
| sm(4)  | \-       | \-                                   | 16                                | 93                      | \-                   | \-                         | 65.09                   | 248             | 29            |
| 21     | inc(2)   | 8                                    | 30                                | 11                      | 41                   | 8                          | 30                      | 1.28            | 37            | 129             | 25              |
| sm(2)  | \-       | \-                                   | 11                                | 41                      | \-                   | \-                         | 58.36                   | 159             | 24            |
| inc(3) | 16       | 77                                   | 20                                | 94                      | 16                   | 77                         | 5.05                    | 241             | 31            |
| sm(3)  | \-       | \-                                   | 14                                | 66                      | \-                   | \-                         | 63.48                   | 260             | 29            |
| inc(4) | 22       | 112                                  | 30                                | 160                     | 20                   | 96                         | 15.79                   | 355             | 36            |
| sm(4)  | \-       | \-                                   | 19                                | 108                     | \-                   | \-                         | 74.05                   | 294             | 37            |
| 17     | inc(2)   | 10                                   | 34                                | 11                      | 38                   | 10                         | 34                      | 0.90            | 35            | 107             | 21              |
| sm(2)  | \-       | \-                                   | 11                                | 38                      | \-                   | \-                         | 60.69                   | 147             | 24            |
| inc(3) | 17       | 74                                   | 19                                | 85                      | 17                   | 74                         | 2.04                    | 188             | 27            |
| sm(3)  | \-       | \-                                   | 14                                | 62                      | \-                   | \-                         | 62.25                   | 233             | 28            |
| inc(4) | 23       | 109                                  | 24                                | 113                     | 23                   | 109                        | 3.3                     | 266             | 33            |
| sm(4)  | \-       | \-                                   | 17                                | 97                      | \-                   | \-                         | 88.03                   | 282             | 32            |
| 40     | inc(2)   | 10                                   | 34                                | 12                      | 38                   | 10                         | 34                      | 1.16            | 34            | 121             | 23              |
| sm(2)  | \-       | \-                                   | 12                                | 38                      | \-                   | \-                         | 56.74                   | 115             | 21            |
| inc(3) | 18       | 81                                   | 20                                | 85                      | 18                   | 81                         | 3.42                    | 228             | 32            |
| sm(3)  | \-       | \-                                   | 15                                | 62                      | \-                   | \-                         | 65.37                   | 220             | 30            |
| inc(4) | 23       | 111                                  | 26                                | 120                     | 22                   | 99                         | 7.01                    | 273             | 33            |
| sm(4)  | \-       | \-                                   | 16                                | 93                      | \-                   | \-                         | 76.16                   | 229             | 26            |
| 23     | inc(2)   | 10                                   | 36                                | 13                      | 47                   | 10                         | 36                      | 1.69            | 41            | 159             | 31              |
| sm(2)  | \-       | \-                                   | 14                                | 49                      | \-                   | \-                         | 56.49                   | 157             | 26            |
| inc(3) | 18       | 83                                   | 22                                | 100                     | 18                   | 83                         | 6.54                    | 266             | 38            |
| sm(3)  | \-       | \-                                   | 17                                | 74                      | \-                   | \-                         | 69.36                   | 227             | 34            |
| inc(4) | 23       | 113                                  | 31                                | 147                     | 22                   | 101                        | 16.69                   | 331             | 39            |
| sm(4)  | \-       | \-                                   | 20                                | 112                     | \-                   | \-                         | 70.03                   | 304             | 37            |
| 22     | inc(2)   | 10                                   | 38                                | 12                      | 42                   | 10                         | 38                      | 1.43            | 38            | 123             | 25              |
| sm(2)  | \-       | \-                                   | 13                                | 45                      | \-                   | \-                         | 57.95                   | 137             | 24            |
| inc(3) | 18       | 79                                   | 21                                | 90                      | 18                   | 79                         | 3.73                    | 223             | 32            |
| sm(3)  | \-       | \-                                   | 16                                | 70                      | \-                   | \-                         | 68.37                   | 228             | 31            |
| inc(4) | 26       | 127                                  | 27                                | 126                     | 24                   | 113                        | 5.84                    | 309             | 37            |
| sm(4)  | \-       | \-                                   | 19                                | 108                     | \-                   | \-                         | 66.25                   | 273             | 34            |
| 25     | inc(2)   | 5                                    | 19                                | 7                       | 23                   | 5                          | 19                      | 1.07            | 19            | 69              | 13              |
| sm(2)  | \-       | \-                                   | 7                                 | 23                      | \-                   | \-                         | 56.71                   | 69              | 13            |
| inc(3) | 9        | 46                                   | 11                                | 50                      | 9                    | 46                         | 3.24                    | 161             | 19            |
| sm(3)  | \-       | \-                                   | 8                                 | 40                      | \-                   | \-                         | 62.93                   | 171             | 19            |
| inc(4) | 9        | 46                                   | 11                                | 50                      | 9                    | 46                         | 4.53                    | 161             | 19            |
| sm(4)  | \-       | \-                                   | 4                                 | 32                      | \-                   | \-                         | 53.98                   | 153             | 18            |
| 30     | inc(2)   | 5                                    | 19                                | 6                       | 21                   | 5                          | 19                      | 0.71            | 20            | 75              | 14              |
| sm(2)  | \-       | \-                                   | 6                                 | 21                      | \-                   | \-                         | 61.37                   | 75              | 14            |
| inc(3) | 8        | 39                                   | 10                                | 52                      | 8                    | 39                         | 2.64                    | 167             | 20            |
| sm(3)  | \-       | \-                                   | 8                                 | 40                      | \-                   | \-                         | 57.28                   | 209             | 19            |
| inc(4) | 9        | 46                                   | 11                                | 62                      | 9                    | 46                         | 3.85                    | 185             | 20            |
| sm(4)  | \-       | \-                                   | 7                                 | 47                      | \-                   | \-                         | 62.7                    | 220             | 19            |
| 26     | inc(2)   | 7                                    | 23                                | 8                       | 27                   | 7                          | 23                      | 1.11            | 21            | 84              | 17              |
| sm(2)  | \-       | \-                                   | 8                                 | 27                      | \-                   | \-                         | 59.68                   | 84              | 17            |
| inc(3) | 10       | 43                                   | 11                                | 47                      | 10                   | 43                         | 1.91                    | 141             | 21            |
| sm(3)  | \-       | \-                                   | 9                                 | 44                      | \-                   | \-                         | 62.04                   | 158             | 21            |
| inc(4) | 10       | 43                                   | 11                                | 47                      | 10                   | 43                         | 4.35                    | 141             | 21            |
| sm(4)  | \-       | \-                                   | 5                                 | 36                      | \-                   | \-                         | 60.81                   | 143             | 17            |
| 28     | inc(2)   | 7                                    | 23                                | 8                       | 25                   | 7                          | 23                      | 0.73            | 21            | 70              | 15              |
| sm(2)  | \-       | \-                                   | 8                                 | 25                      | \-                   | \-                         | 62.82                   | 110             | 16            |
| inc(3) | 10       | 43                                   | 13                                | 58                      | 10                   | 43                         | 2.66                    | 157             | 20            |
| sm(3)  | \-       | \-                                   | 10                                | 44                      | \-                   | \-                         | 80.96                   | 195             | 20            |
| inc(4) | 11       | 50                                   | 14                                | 68                      | 11                   | 50                         | 3.76                    | 181             | 21            |
| sm(4)  | \-       | \-                                   | 7                                 | 47                      | \-                   | \-                         | 71.63                   | 145             | 18            |
| 32     | inc(2)   | 7                                    | 25                                | 8                       | 27                   | 7                          | 25                      | 0.98            | 24            | 81              | 16              |
| sm(2)  | \-       | \-                                   | 9                                 | 29                      | \-                   | \-                         | 55.46                   | 83              | 16            |
| inc(3) | 11       | 52                                   | 12                                | 58                      | 11                   | 52                         | 2.03                    | 152             | 21            |
| sm(3)  | \-       | \-                                   | 11                                | 48                      | \-                   | \-                         | 63.97                   | 194             | 20            |
| inc(4) | 11       | 52                                   | 13                                | 68                      | 11                   | 52                         | 4.16                    | 182             | 23            |
| sm(4)  | \-       | \-                                   | 8                                 | 51                      | \-                   | \-                         | 68.32                   | 179             | 23            |
| 38     | inc(2)   | 8                                    | 27                                | 9                       | 29                   | 8                          | 27                      | 0.55            | 26            | 77              | 18              |
| sm(2)  | \-       | \-                                   | 10                                | 31                      | \-                   | \-                         | 56.57                   | 93              | 19            |
| inc(3) | 13       | 60                                   | 14                                | 66                      | 13                   | 60                         | 2.25                    | 155             | 23            |
| sm(3)  | \-       | \-                                   | 13                                | 52                      | \-                   | \-                         | 61.46                   | 177             | 25            |
| inc(4) | 13       | 59                                   | 16                                | 82                      | 13                   | 59                         | 4.28                    | 205             | 26            |
| sm(4)  | \-       | \-                                   | 11                                | 66                      | \-                   | \-                         | 69.45                   | 176             | 21            |
| 33     | inc(2)   | 6                                    | 21                                | 9                       | 32                   | 6                          | 21                      | 2..55           | 31            | 112             | 24              |
| sm(2)  | \-       | \-                                   | 9                                 | 32                      | \-                   | \-                         | 57.63                   | 116             | 24            |
| inc(3) | 10       | 47                                   | 16                                | 85                      | 10                   | 47                         | 5.92                    | 242             | 28            |
| sm(3)  | \-       | \-                                   | 11                                | 54                      | \-                   | \-                         | 64.24                   | 219             | 30            |
| inc(4) | 12       | 60                                   | 21                                | 121                     | 12                   | 60                         | 17.89                   | 310             | 31            |
| sm(4)  | \-       | \-                                   | 13                                | 78                      | \-                   | \-                         | 65.74                   | 232             | 30            |
| 35     | inc(2)   | 8                                    | 27                                | 11                      | 38                   | 8                          | 27                      | 3.01            | 34            | 127             | 23              |
| sm(2)  | \-       | \-                                   | 12                                | 40                      | \-                   | \-                         | 63.54                   | 156             | 25            |
| inc(3) | 13       | 60                                   | 18                                | 91                      | 13                   | 60                         | 7.32                    | 254             | 30            |
| sm(3)  | \-       | \-                                   | 14                                | 62                      | \-                   | \-                         | 64.61                   | 210             | 29            |
| inc(4) | 14       | 66                                   | 25                                | 138                     | 14                   | 66                         | 20.66                   | 327             | 33            |
| sm(4)  | \-       | \-                                   | 14                                | 82                      | \-                   | \-                         | 66.87                   | 239             | 27            |
| 34     | inc(2)   | 9                                    | 32                                | 11                      | 36                   | 9                          | 32                      | 1.03            | 32            | 117             | 25              |
| sm(2)  | \-       | \-                                   | 11                                | 36                      | \-                   | \-                         | 58.66                   | 141             | 25            |
| inc(3) | 16       | 73                                   | 18                                | 77                      | 16                   | 73                         | 3.29                    | 207             | 29            |
| sm(3)  | \-       | \-                                   | 13                                | 58                      | \-                   | \-                         | 63.23                   | 240             | 31            |
| inc(4) | 21       | 102                                  | 23                                | 106                     | 19                   | 86                         | 5.22                    | 266             | 32            |
| sm(4)  | \-       | \-                                   | 13                                | 78                      | \-                   | \-                         | 63.83                   | 237             | 29            |
| 39     | inc(2)   | 9                                    | 32                                | 10                      | 34                   | 9                          | 32                      | 0.86            | 33            | 124             | 23              |
| sm(2)  | \-       | \-                                   | 10                                | 34                      | \-                   | \-                         | 57.47                   | 128             | 22            |
| inc(3) | 15       | 66                                   | 18                                | 81                      | 15                   | 66                         | 2.41                    | 232             | 31            |
| sm(3)  | \-       | \-                                   | 13                                | 58                      | \-                   | \-                         | 64.56                   | 241             | 30            |
| inc(4) | 20       | 95                                   | 23                                | 113                     | 18                   | 78                         | 4.49                    | 278             | 32            |
| sm(4)  | \-       | \-                                   | 16                                | 93                      | \-                   | \-                         | 75.41                   | 244             | 29            |
| 41     | inc(2)   | 11                                   | 38                                | 12                      | 40                   | 11                         | 38                      | 0.66            | 37            | 110             | 22              |
| sm(2)  | \-       | \-                                   | 13                                | 42                      | \-                   | \-                         | 61.66                   | 139             | 23            |
| inc(3) | 17       | 72                                   | 19                                | 80                      | 17                   | 72                         | 2.70                    | 199             | 29            |
| sm(3)  | \-       | \-                                   | 16                                | 66                      | \-                   | \-                         | 67.75                   | 228             | 31            |
| inc(4) | 22       | 101                                  | 26                                | 126                     | 19                   | 79                         | 4.02                    | 297             | 35            |
| sm(4)  | \-       | \-                                   | 17                                | 97                      | \-                   | \-                         | 66.14                   | 275             | 32            |
