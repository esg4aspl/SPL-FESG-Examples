# Bank Account Product Line
Bank account product line has 9 features and a core feature. The core of the product line represents the common behavior which exists in all products that belong to bank account product line. The core behavior is modelled using core ESG (c-ESG). An optional behavior is modelled using a feature ESG (f-ESG). A featured ESG (FESG) is an extended ESG that is composed of a core ESG (c-ESG) and a set of feature ESGs (f-ESGs). A featured ESG is used in test sequence composition approach which composes the sequences of core and feature ESGs and generates a product's test sequences. The models of bank account product line are built from the users' perspective. The Event Sequence graphs' events are selected from user events. 

## Feature Model
![Feature Model](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_ModelImages/BankAccountPL_featureModel.PNG)

This feature model has 2 mandatory and 7 optional features. The feature _interest estimation_ implies _interest_; _daily limit_ implies _withdraw_ and _cancel withdraw_ and, _overdraft_ implies _cancel withdraw_ and _daily limit_. This means that a product configuration which has one of the implying features i.e. cancel withdraw, interest estimation etc. must have the corresponding implied feature. 42 different product configurations could be obtained by combining these features. 

## Bank Account Products
![Full Product Matrix](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_ModelImages/BankAccountPL_fullProductMatrix.png)

The full product matrix demonstrates the product configurations of the Bank Account Product Line feature model. There are 42 product configurations. In the table below, the product id and the belonging features are given. The products are assigned with a unique ID since, each possible product does not have a unique official name.

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

 [Click for the PDF version of the table](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/Products.pdf)

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
Interest Product has interest feature additional to the mandatory features. The users of this product can request an interest rate and confirm it if it is suitable. \
[Interest Product ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_Models/BankAccountPLProduct_Interest.zip)

[Click to download all ESG MXE Files](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/BankAccountPL_Models/BankAccountPL_Models.zip)

  # Bank Account Product Line Experiments and Results
The Bank Account Product Line has forty two(42) product configurations and ninty seven(97) one-increment i.e., one feature addition, testing scenarios in total. In our study, we select 30 of the testing scenarios randomly. In the selection process of the one increment scenarios, the following two rules are applied:
1. The same scenario has not been selected more than once.
2. The same PUC has not been selected more than twice.

## Testing Scenarios
In this table, the selected testing scenarios are given with their Scenario IDs, Product Under Consideration(PUC) IDs, Existing Product IDs and Features and Increment. Existing Product refers to the product that we already have the model and the test sequences. In incremental test generation approach, the existing product's test sequences and increment's test sequences are composed so that the test sequences of the PUC is obtained without generating and composing all of its features from scratch.

| Scenario ID | Product Under Consideration ID | Existing Product ID | Existing Product Features                                                                  | New Feature        |
| ----------- | ------------------------------ | ------------------- | ------------------------------------------------------------------------------------------ | ------------------ |
| 4           | 2                              | 1                   | deposit, withdraw, interest                                                                | interestEstimation |
| 5           | 4                              | 1                   | deposit, withdraw, interest                                                                | cancelDeposit      |
| 2           | 6                              | 0                   | deposit, withdraw                                                                          | cancelWithdraw     |
| 19          | 7                              | 6                   | deposit, withdraw, cancelWithdraw                                                          | interest           |
| 23          | 8                              | 7                   | deposit, withdraw, interest, cancelWithdraw                                                | interestEstimation |
| 20          | 9                              | 6                   | deposit, withdraw, cancelWithdraw                                                          | dailyLimit         |
| 41          | 13                             | 12                  | deposit, withdraw, cancelDeposit, cancelWithdraw                                           | interest           |
| 17          | 14                             | 5                   | deposit, withdraw, cancelDeposit, interest, interestEstimation                             | cancelWithdraw     |
| 31          | 15                             | 9                   | deposit, withdraw, cancelWithdraw, dailyLimit                                              | cancelDeposit      |
| 49          | 16                             | 15                  | deposit, withdraw, cancelDeposit, cancelWithdraw, dailyLimit                               | interest           |
| 52          | 17                             | 16                  | deposit, withdraw, cancelDeposit, interest, cancelWithdraw, dailyLimit                     | interestEstimation |
| 36          | 19                             | 10                  | deposit, withdraw, interest, cancelWithdraw, dailyLimit                                    | overdraft          |
| 39          | 20                             | 11                  | deposit, withdraw, interest, cancelWithdraw, dailyLimit, interestEstimation                | overdraft          |
| 50          | 21                             | 15                  | deposit, withdraw, cancelDeposit, cancelWithdraw, dailyLimit                               | overdraft          |
| 62          | 22                             | 21                  | deposit, withdraw, cancelDeposit, cancelWithdraw, dailyLimit, overdraft                    | interest           |
| 55          | 23                             | 17                  | deposit, withdraw, cancelDeposit, interest, cancelWithdraw, dailyLimit, interestEstimation | overdraft          |
| 3           | 24                             | 0                   | deposit, withdraw                                                                          | credit             |
| 64          | 25                             | 24                  | deposit, withdraw, credit                                                                  | interest           |
| 67          | 26                             | 25                  | deposit, withdraw, credit, interest                                                        | interestEstimation |
| 68          | 28                             | 25                  | deposit, withdraw, credit, interest                                                        | cancelDeposit      |
| 66          | 30                             | 24                  | deposit, withdraw, credit                                                                  | cancelWithdraw     |
| 71          | 32                             | 26                  | deposit, withdraw, credit, interest, interestEstimation                                    | cancelWithdraw     |
| 78          | 33                             | 30                  | deposit, withdraw, credit, cancelWithdraw                                                  | dailyLimit         |
| 85          | 34                             | 33                  | deposit, withdraw, credit, cancelWithdraw, dailyLimit                                      | interest           |
| 83          | 35                             | 32                  | deposit, withdraw, credit, interest, cancelWithdraw, interestEstimation                    | dailyLimit         |
| 43          | 36                             | 12                  | deposit, withdraw, cancelDeposit, cancelWithdraw                                           | credit             |
| 76          | 38                             | 29                  | deposit, withdraw, cancelDeposit, credit, interest, interestEstimation                     | cancelWithdraw     |
| 86          | 39                             | 33                  | deposit, withdraw, credit, cancelWithdraw, dailyLimit                                      | cancelDeposit      |
| 54          | 40                             | 16                  | deposit, withdraw, cancelDeposit, interest, cancelWithdraw, dailyLimit                     | credit             |
| 89          | 41                             | 35                  | deposit, withdraw, credit, interest, cancelWithdraw, dailyLimit, interestEstimation        | cancelDeposit      |

[Click for the PDF version of the table](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/Testing%20Scenarios.pdf)

## Data on PUCs
The numbers of k-sequences where k=1,2,3,4 are given to give a notion of the sizes of the selected PUCs in the testing scenarios.

| Product Under Consideration ID | k = 1 |  k = 2 | k = 3 | k = 4 |
| ------------------------------ | ----- | ------ | ----- | ----- |
| 6                              | 8     | 9      | 11    | 14    |
| 24                             | 10    | 10     | 10    | 12    |
| 2                              | 12    | 12     | 12    | 13    |
| 4                              | 11    | 11     | 11    | 14    |
| 14                             | 14    | 14     | 14    | 17    |
| 7                              | 11    | 11     | 11    | 14    |
| 9                              | 10    | 13     | 17    | 23    |
| 8                              | 13    | 13     | 13    | 15    |
| 15                             | 11    | 14     | 18    | 25    |
| 19                             | 15    | 18     | 20    | 27    |
| 20                             | 17    | 20     | 22    | 28    |
| 13                             | 12    | 12     | 12    | 16    |
| 36                             | 12    | 12     | 12    | 16    |
| 16                             | 14    | 16     | 18    | 25    |
| 21                             | 13    | 17     | 21    | 29    |
| 17                             | 16    | 18     | 20    | 26    |
| 40                             | 17    | 18     | 18    | 25    |
| 23                             | 18    | 21     | 23    | 30    |
| 22                             | 16    | 19     | 21    | 29    |
| 25                             | 13    | 12     | 10    | 12    |
| 30                             | 11    | 11     | 11    | 14    |
| 26                             | 15    | 14     | 12    | 13    |
| 28                             | 14    | 13     | 11    | 14    |
| 32                             | 16    | 15     | 13    | 15    |
| 38                             | 17    | 16     | 14    | 17    |
| 33                             | 13    | 15     | 17    | 23    |
| 35                             | 18    | 19     | 19    | 24    |
| 34                             | 16    | 17     | 17    | 23    |
| 39                             | 14    | 16     | 18    | 25    |
| 41                             | 19    | 20     | 20    | 26    |

[Click for the PDF version of the table](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/Data%20on%20PUCs.pdf)

## Data on Number of Faults
The table below contains the total number of possible faults and the number of faults seeded for various m values for each PUC. The entire number of possible faults for each PUC for a given value of m is directly proportional to the number of m-sequences in the PUC's ESG, and the total number of seeded faults is 20% of the summation of number of possible faults for m=2,3,4,5.

| Scenario ID | PUC ID | m=2 | m=3 | m=4 | m=5 | Total Number of Possible Faults | Number of Seeded Faults |
| ----------- | ------ | --- | --- | --- | --- | ------------------------------- | ----------------------- |
| 2           | 6      | 17  | 20  | 25  | 30  | 92                              | 18                      |
| 3           | 24     | 20  | 20  | 22  | 26  | 88                              | 18                      |
| 4           | 2      | 24  | 24  | 25  | 27  | 100                             | 20                      |
| 5           | 4      | 22  | 22  | 25  | 30  | 99                              | 20                      |
| 17          | 14     | 28  | 28  | 31  | 35  | 122                             | 24                      |
| 19          | 7      | 22  | 22  | 25  | 30  | 99                              | 20                      |
| 20          | 9      | 23  | 30  | 40  | 53  | 146                             | 29                      |
| 23          | 8      | 26  | 26  | 28  | 31  | 111                             | 22                      |
| 31          | 15     | 25  | 32  | 43  | 57  | 157                             | 31                      |
| 36          | 19     | 33  | 38  | 47  | 62  | 180                             | 36                      |
| 39          | 20     | 37  | 42  | 50  | 63  | 192                             | 38                      |
| 41          | 13     | 24  | 24  | 28  | 34  | 110                             | 22                      |
| 43          | 36     | 24  | 24  | 28  | 34  | 110                             | 22                      |
| 49          | 16     | 30  | 34  | 43  | 57  | 164                             | 33                      |
| 50          | 21     | 30  | 38  | 50  | 66  | 184                             | 37                      |
| 52          | 17     | 34  | 38  | 46  | 58  | 176                             | 35                      |
| 54          | 40     | 35  | 36  | 43  | 57  | 171                             | 34                      |
| 55          | 23     | 39  | 44  | 53  | 67  | 203                             | 41                      |
| 62          | 22     | 35  | 40  | 50  | 66  | 191                             | 38                      |
| 64          | 25     | 25  | 22  | 22  | 26  | 95                              | 19                      |
| 66          | 30     | 22  | 22  | 25  | 30  | 99                              | 20                      |
| 67          | 26     | 29  | 26  | 25  | 27  | 107                             | 21                      |
| 68          | 28     | 27  | 24  | 25  | 30  | 106                             | 21                      |
| 71          | 32     | 31  | 28  | 28  | 31  | 118                             | 24                      |
| 76          | 38     | 33  | 30  | 31  | 35  | 129                             | 26                      |
| 78          | 33     | 28  | 32  | 40  | 53  | 153                             | 31                      |
| 83          | 35     | 37  | 38  | 43  | 54  | 172                             | 34                      |
| 85          | 34     | 33  | 34  | 40  | 53  | 160                             | 32                      |
| 86          | 39     | 30  | 34  | 43  | 57  | 164                             | 33                      |
| 89          | 41     | 39  | 40  | 46  | 58  | 183                             | 37                      |

[Click for the PDF version of the table](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/Data%20on%20Number%20of%20Faults.pdf)

## Data on Test Generation and Execution
Table below presents data on fault coverage and performance statistics on test set generation and test execution processes.

| Scenario ID | PUC ID | Test Set | EP Test Set Size | Length of EP Test Set | PUC Test Set Size | Length of PUC Test Set | Test Sequences Reused in Test Set | Events Reused in Test Sequences | Generation Time | Faults Seeded | Events Executed | Faults Revealed |
| ----------- | ------ | -------- | ---------------- | --------------------- | ----------------- | ---------------------- | --------------------------------- | ------------------------------- | --------------- | ------------- | --------------- | --------------- |
| 2           | 6      | inc(2)   | 3                | 15                    | 4                 | 17                     | 3                                 | 15                              | 0.8             | 18            | 67              | 13              |
| 2           | 6      | sm(2)    | \-               | \-                    | 4                 | 17                     | \-                                | \-                              | 64.11           | 18            | 67              | 13              |
| 2           | 6      | inc(3)   | 5                | 32                    | 7                 | 45                     | 5                                 | 32                              | 2.69            | 18            | 151             | 18              |
| 2           | 6      | sm(3)    | \-               | \-                    | 6                 | 36                     | \-                                | \-                              | 66.81           | 18            | 148             | 18              |
| 2           | 6      | inc(4)   | 6                | 39                    | 8                 | 55                     | 6                                 | 39                              | 6.47            | 18            | 173             | 18              |
| 2           | 6      | sm(4)    | \-               | \-                    | 7                 | 47                     | \-                                | \-                              | 69.11           | 18            | 205             | 18              |
| 3           | 24     | inc(2)   | 3                | 15                    | 5                 | 19                     | 3                                 | 15                              | 1.45            | 18            | 56              | 13              |
| 3           | 24     | sm(2)    | \-               | \-                    | 5                 | 19                     | \-                                | \-                              | 63.01           | 18            | 56              | 13              |
| 3           | 24     | inc(3)   | 5                | 32                    | 8                 | 43                     | 5                                 | 32                              | 2.86            | 18            | 131             | 18              |
| 3           | 24     | sm(3)    | \-               | \-                    | 6                 | 36                     | \-                                | \-                              | 58.64           | 18            | 164             | 18              |
| 3           | 24     | inc(4)   | 6                | 39                    | 8                 | 43                     | 6                                 | 39                              | 3.98            | 18            | 131             | 18              |
| 3           | 24     | sm(4)    | \-               | \-                    | 4                 | 32                     | \-                                | \-                              | 57.8            | 18            | 128             | 16              |
| 4           | 2      | inc(2)   | 5                | 19                    | 6                 | 23                     | 5                                 | 19                              | 0.83            | 20            | 78              | 16              |
| 4           | 2      | sm(2)    | \-               | \-                    | 6                 | 23                     | \-                                | \-                              | 75.56           | 20            | 78              | 16              |
| 4           | 2      | inc(3)   | 8                | 39                    | 9                 | 43                     | 8                                 | 39                              | 2.01            | 20            | 159             | 20              |
| 4           | 2      | sm(3)    | \-               | \-                    | 7                 | 40                     | \-                                | \-                              | 67.29           | 20            | 160             | 20              |
| 4           | 2      | inc(4)   | 8                | 39                    | 9                 | 43                     | 8                                 | 39                              | 4.07            | 20            | 159             | 20              |
| 4           | 2      | sm(4)    | \-               | \-                    | 5                 | 36                     | \-                                | \-                              | 73.28           | 20            | 156             | 20              |
| 5           | 4      | inc(2)   | 5                | 19                    | 6                 | 21                     | 5                                 | 19                              | 0.99            | 20            | 68              | 13              |
| 5           | 4      | sm(2)    | \-               | \-                    | 6                 | 21                     | \-                                | \-                              | 52.38           | 20            | 84              | 13              |
| 5           | 4      | inc(3)   | 8                | 39                    | 11                | 54                     | 8                                 | 39                              | 2.2             | 20            | 149             | 19              |
| 5           | 4      | sm(3)    | \-               | \-                    | 8                 | 40                     | \-                                | \-                              | 63.49           | 20            | 191             | 19              |
| 5           | 4      | inc(4)   | 8                | 39                    | 12                | 64                     | 8                                 | 39                              | 6.57            | 20            | 169             | 20              |
| 5           | 4      | sm(4)    | \-               | \-                    | 7                 | 47                     | \-                                | \-                              | 61.36           | 20            | 142             | 17              |
| 17          | 14     | inc(2)   | 6                | 23                    | 7                 | 25                     | 6                                 | 23                              | 0.82            | 24            | 68              | 16              |
| 17          | 14     | sm(2)    | \-               | \-                    | 8                 | 27                     | \-                                | \-                              | 55.26           | 24            | 128             | 20              |
| 17          | 14     | inc(3)   | 10               | 49                    | 12                | 62                     | 10                                | 49                              | 2.61            | 24            | 157             | 21              |
| 17          | 14     | sm(3)    | \-               | \-                    | 11                | 48                     | \-                                | \-                              | 68.64           | 24            | 163             | 23              |
| 17          | 14     | inc(4)   | 12               | 62                    | 14                | 78                     | 12                                | 62                              | 3.85            | 24            | 199             | 24              |
| 17          | 14     | sm(4)    | \-               | \-                    | 11                | 66                     | \-                                | \-                              | 69.48           | 24            | 175             | 24              |
| 19          | 7      | inc(2)   | 4                | 17                    | 6                 | 21                     | 4                                 | 17                              | 1.2             | 20            | 75              | 14              |
| 19          | 7      | sm(2)    | \-               | \-                    | 6                 | 21                     | \-                                | \-                              | 56.06           | 20            | 75              | 14              |
| 19          | 7      | inc(3)   | 8                | 43                    | 11                | 54                     | 8                                 | 43                              | 2.96            | 20            | 161             | 20              |
| 19          | 7      | sm(3)    | \-               | \-                    | 8                 | 40                     | \-                                | \-                              | 61.87           | 20            | 209             | 19              |
| 19          | 7      | inc(4)   | 10               | 56                    | 12                | 60                     | 10                                | 56                              | 3.63            | 20            | 175             | 20              |
| 19          | 7      | sm(4)    | \-               | \-                    | 7                 | 47                     | \-                                | \-                              | 66.43           | 20            | 220             | 19              |
| 20          | 9      | inc(2)   | 4                | 17                    | 7                 | 28                     | 4                                 | 17                              | 2.43            | 29            | 110             | 24              |
| 20          | 9      | sm(2)    | \-               | \-                    | 7                 | 28                     | \-                                | \-                              | 51.31           | 29            | 118             | 24              |
| 20          | 9      | inc(3)   | 8                | 43                    | 14                | 81                     | 8                                 | 43                              | 7.46            | 29            | 239             | 26              |
| 20          | 9      | sm(3)    | \-               | \-                    | 9                 | 50                     | \-                                | \-                              | 63.17           | 29            | 244             | 28              |
| 20          | 9      | inc(4)   | 10               | 56                    | 20                | 126                    | 10                                | 56                              | 14.57           | 29            | 310             | 29              |
| 20          | 9      | sm(4)    | \-               | \-                    | 13                | 78                     | \-                                | \-                              | 70.92           | 29            | 230             | 29              |
| 23          | 8      | inc(2)   | 6                | 21                    | 7                 | 25                     | 6                                 | 21                              | 0.94            | 22            | 77              | 16              |
| 23          | 8      | sm(2)    | \-               | \-                    | 7                 | 25                     | \-                                | \-                              | 71.48           | 22            | 83              | 17              |
| 23          | 8      | inc(3)   | 11               | 54                    | 11                | 51                     | 10                                | 47                              | 2.02            | 22            | 141             | 20              |
| 23          | 8      | sm(3)    | \-               | \-                    | 9                 | 44                     | \-                                | \-                              | 55.89           | 22            | 164             | 19              |
| 23          | 8      | inc(4)   | 11               | 53                    | 12                | 57                     | 11                                | 53                              | 3.23            | 22            | 159             | 22              |
| 23          | 8      | sm(4)    | \-               | \-                    | 8                 | 51                     | \-                                | \-                              | 59.05           | 22            | 147             | 21              |
| 31          | 15     | inc(2)   | 7                | 28                    | 8                 | 30                     | 7                                 | 28                              | 0.82            | 31            | 128             | 23              |
| 31          | 15     | sm(2)    | \-               | \-                    | 8                 | 30                     | \-                                | \-                              | 52.44           | 31            | 147             | 21              |
| 31          | 15     | inc(3)   | 13               | 62                    | 16                | 77                     | 13                                | 62                              | 2.45            | 31            | 240             | 29              |
| 31          | 15     | sm(3)    | \-               | \-                    | 11                | 54                     | \-                                | \-                              | 63.85           | 31            | 255             | 28              |
| 31          | 15     | inc(4)   | 18               | 91                    | 21                | 109                    | 18                                | 91                              | 3.67            | 31            | 286             | 30              |
| 31          | 15     | sm(4)    | \-               | \-                    | 16                | 93                     | \-                                | \-                              | 69.81           | 31            | 247             | 29              |
| 36          | 19     | inc(2)   | 9                | 32                    | 12                | 43                     | 9                                 | 32                              | 1.7             | 36            | 115             | 23              |
| 36          | 19     | sm(2)    | \-               | \-                    | 12                | 43                     | \-                                | \-                              | 58.12           | 36            | 131             | 23              |
| 36          | 19     | inc(3)   | 15               | 66                    | 20                | 90                     | 15                                | 66                              | 5.76            | 36            | 204             | 30              |
| 36          | 19     | sm(3)    | \-               | \-                    | 14                | 66                     | \-                                | \-                              | 61.61           | 36            | 209             | 27              |
| 36          | 19     | inc(4)   | 20               | 95                    | 27                | 127                    | 18                                | 78                              | 17.76           | 36            | 283             | 34              |
| 36          | 19     | sm(4)    | \-               | \-                    | 16                | 93                     | \-                                | \-                              | 65.83           | 36            | 259             | 28              |
| 39          | 20     | inc(2)   | 9                | 34                    | 12                | 45                     | 9                                 | 34                              | 1.44            | 38            | 155             | 30              |
| 39          | 20     | sm(2)    | \-               | \-                    | 13                | 47                     | \-                                | \-                              | 63.00           | 38            | 157             | 30              |
| 39          | 20     | inc(3)   | 16               | 75                    | 20                | 92                     | 16                                | 75                              | 6.38            | 38            | 258             | 36              |
| 39          | 20     | sm(3)    | \-               | \-                    | 15                | 70                     | \-                                | \-                              | 72.99           | 38            | 237             | 34              |
| 39          | 20     | inc(4)   | 21               | 104                   | 28                | 133                    | 19                                | 87                              | 16.87           | 38            | 305             | 37              |
| 39          | 20     | sm(4)    | \-               | \-                    | 17                | 97                     | \-                                | \-                              | 71.67           | 38            | 234             | 35              |
| 41          | 13     | inc(2)   | 5                | 19                    | 7                 | 23                     | 5                                 | 19                              | 1.32            | 22            | 71              | 14              |
| 41          | 13     | sm(2)    | \-               | \-                    | 7                 | 23                     | \-                                | \-                              | 55.55           | 22            | 81              | 15              |
| 41          | 13     | inc(3)   | 10               | 51                    | 13                | 62                     | 10                                | 51                              | 2.75            | 22            | 170             | 20              |
| 41          | 13     | sm(3)    | \-               | \-                    | 10                | 44                     | \-                                | \-                              | 63.43           | 22            | 164             | 20              |
| 41          | 13     | inc(4)   | 13               | 70                    | 15                | 74                     | 13                                | 70                              | 4.15            | 22            | 198             | 22              |
| 41          | 13     | sm(4)    | \-               | \-                    | 10                | 62                     | \-                                | \-                              | 57.68           | 22            | 196             | 21              |
| 43          | 36     | inc(2)   | 5                | 19                    | 7                 | 23                     | 5                                 | 19                              | 1.21            | 22            | 71              | 14              |
| 43          | 36     | sm(2)    | \-               | \-                    | 7                 | 23                     | \-                                | \-                              | 55.55           | 22            | 81              | 15              |
| 43          | 36     | inc(3)   | 10               | 51                    | 13                | 62                     | 10                                | 51                              | 2.55            | 22            | 170             | 20              |
| 43          | 36     | sm(3)    | \-               | \-                    | 10                | 44                     | \-                                | \-                              | 63.43           | 22            | 164             | 20              |
| 43          | 36     | inc(4)   | 13               | 70                    | 15                | 74                     | 13                                | 70                              | 3.92            | 22            | 198             | 22              |
| 43          | 36     | sm(4)    | \-               | \-                    | 10                | 62                     | \-                                | \-                              | 57.68           | 22            | 188             | 21              |
| 49          | 16     | inc(2)   | 8                | 30                    | 10                | 34                     | 8                                 | 30                              | 1.14            | 33            | 124             | 23              |
| 49          | 16     | sm(2)    | \-               | \-                    | 10                | 34                     | \-                                | \-                              | 55.94           | 33            | 128             | 22              |
| 49          | 16     | inc(3)   | 16               | 77                    | 18                | 81                     | 16                                | 77                              | 2.71            | 33            | 232             | 31              |
| 49          | 16     | sm(3)    | \-               | \-                    | 13                | 58                     | \-                                | \-                              | 62.88           | 33            | 243             | 30              |
| 49          | 16     | inc(4)   | 22               | 112                   | 24                | 116                    | 22                                | 112                             | 4.25            | 33            | 285             | 32              |
| 49          | 16     | sm(4)    | \-               | \-                    | 16                | 93                     | \-                                | \-                              | 65.09           | 33            | 248             | 29              |
| 50          | 21     | inc(2)   | 8                | 30                    | 11                | 41                     | 8                                 | 30                              | 1.28            | 37            | 129             | 25              |
| 50          | 21     | sm(2)    | \-               | \-                    | 11                | 41                     | \-                                | \-                              | 58.36           | 37            | 159             | 24              |
| 50          | 21     | inc(3)   | 16               | 77                    | 20                | 94                     | 16                                | 77                              | 5.05            | 37            | 241             | 31              |
| 50          | 21     | sm(3)    | \-               | \-                    | 14                | 66                     | \-                                | \-                              | 63.48           | 37            | 260             | 29              |
| 50          | 21     | inc(4)   | 22               | 112                   | 30                | 160                    | 20                                | 96                              | 15.79           | 37            | 355             | 36              |
| 50          | 21     | sm(4)    | \-               | \-                    | 19                | 108                    | \-                                | \-                              | 74.05           | 37            | 294             | 37              |
| 52          | 17     | inc(2)   | 10               | 34                    | 11                | 38                     | 10                                | 34                              | 0.90            | 35            | 107             | 21              |
| 52          | 17     | sm(2)    | \-               | \-                    | 11                | 38                     | \-                                | \-                              | 60.69           | 35            | 147             | 24              |
| 52          | 17     | inc(3)   | 17               | 74                    | 19                | 85                     | 17                                | 74                              | 2.04            | 35            | 188             | 27              |
| 52          | 17     | sm(3)    | \-               | \-                    | 14                | 62                     | \-                                | \-                              | 62.25           | 35            | 233             | 28              |
| 52          | 17     | inc(4)   | 23               | 109                   | 24                | 113                    | 23                                | 109                             | 3.3             | 35            | 266             | 33              |
| 52          | 17     | sm(4)    | \-               | \-                    | 17                | 97                     | \-                                | \-                              | 88.03           | 35            | 282             | 32              |
| 54          | 40     | inc(2)   | 10               | 34                    | 12                | 38                     | 10                                | 34                              | 1.16            | 34            | 121             | 23              |
| 54          | 40     | sm(2)    | \-               | \-                    | 12                | 38                     | \-                                | \-                              | 56.74           | 34            | 115             | 21              |
| 54          | 40     | inc(3)   | 18               | 81                    | 20                | 85                     | 18                                | 81                              | 3.42            | 34            | 228             | 32              |
| 54          | 40     | sm(3)    | \-               | \-                    | 15                | 62                     | \-                                | \-                              | 65.37           | 34            | 220             | 30              |
| 54          | 40     | inc(4)   | 23               | 111                   | 26                | 120                    | 22                                | 99                              | 7.01            | 34            | 273             | 33              |
| 54          | 40     | sm(4)    | \-               | \-                    | 16                | 93                     | \-                                | \-                              | 76.16           | 34            | 229             | 26              |
| 55          | 23     | inc(2)   | 10               | 36                    | 13                | 47                     | 10                                | 36                              | 1.69            | 41            | 159             | 31              |
| 55          | 23     | sm(2)    | \-               | \-                    | 14                | 49                     | \-                                | \-                              | 56.49           | 41            | 157             | 26              |
| 55          | 23     | inc(3)   | 18               | 83                    | 22                | 100                    | 18                                | 83                              | 6.54            | 41            | 266             | 38              |
| 55          | 23     | sm(3)    | \-               | \-                    | 17                | 74                     | \-                                | \-                              | 69.36           | 41            | 227             | 34              |
| 55          | 23     | inc(4)   | 23               | 113                   | 31                | 147                    | 22                                | 101                             | 16.69           | 41            | 331             | 39              |
| 55          | 23     | sm(4)    | \-               | \-                    | 20                | 112                    | \-                                | \-                              | 70.03           | 41            | 304             | 37              |
| 62          | 22     | inc(2)   | 10               | 38                    | 12                | 42                     | 10                                | 38                              | 1.43            | 38            | 123             | 25              |
| 62          | 22     | sm(2)    | \-               | \-                    | 13                | 45                     | \-                                | \-                              | 57.95           | 38            | 137             | 24              |
| 62          | 22     | inc(3)   | 18               | 79                    | 21                | 90                     | 18                                | 79                              | 3.73            | 38            | 223             | 32              |
| 62          | 22     | sm(3)    | \-               | \-                    | 16                | 70                     | \-                                | \-                              | 68.37           | 38            | 228             | 31              |
| 62          | 22     | inc(4)   | 26               | 127                   | 27                | 126                    | 24                                | 113                             | 5.84            | 38            | 309             | 37              |
| 62          | 22     | sm(4)    | \-               | \-                    | 19                | 108                    | \-                                | \-                              | 66.25           | 38            | 273             | 34              |
| 64          | 25     | inc(2)   | 5                | 19                    | 7                 | 23                     | 5                                 | 19                              | 1.07            | 19            | 69              | 13              |
| 64          | 25     | sm(2)    | \-               | \-                    | 7                 | 23                     | \-                                | \-                              | 56.71           | 19            | 69              | 13              |
| 64          | 25     | inc(3)   | 9                | 46                    | 11                | 50                     | 9                                 | 46                              | 3.24            | 19            | 161             | 19              |
| 64          | 25     | sm(3)    | \-               | \-                    | 8                 | 40                     | \-                                | \-                              | 62.93           | 19            | 171             | 19              |
| 64          | 25     | inc(4)   | 9                | 46                    | 11                | 50                     | 9                                 | 46                              | 4.53            | 19            | 161             | 19              |
| 64          | 25     | sm(4)    | \-               | \-                    | 4                 | 32                     | \-                                | \-                              | 53.98           | 19            | 153             | 18              |
| 66          | 30     | inc(2)   | 5                | 19                    | 6                 | 21                     | 5                                 | 19                              | 0.71            | 20            | 75              | 14              |
| 66          | 30     | sm(2)    | \-               | \-                    | 6                 | 21                     | \-                                | \-                              | 61.37           | 20            | 75              | 14              |
| 66          | 30     | inc(3)   | 8                | 39                    | 10                | 52                     | 8                                 | 39                              | 2.64            | 20            | 167             | 20              |
| 66          | 30     | sm(3)    | \-               | \-                    | 8                 | 40                     | \-                                | \-                              | 57.28           | 20            | 209             | 19              |
| 66          | 30     | inc(4)   | 9                | 46                    | 11                | 62                     | 9                                 | 46                              | 3.85            | 20            | 185             | 20              |
| 66          | 30     | sm(4)    | \-               | \-                    | 7                 | 47                     | \-                                | \-                              | 62.7            | 20            | 220             | 19              |
| 67          | 26     | inc(2)   | 7                | 23                    | 8                 | 27                     | 7                                 | 23                              | 1.11            | 21            | 84              | 17              |
| 67          | 26     | sm(2)    | \-               | \-                    | 8                 | 27                     | \-                                | \-                              | 59.68           | 21            | 84              | 17              |
| 67          | 26     | inc(3)   | 10               | 43                    | 11                | 47                     | 10                                | 43                              | 1.91            | 21            | 141             | 21              |
| 67          | 26     | sm(3)    | \-               | \-                    | 9                 | 44                     | \-                                | \-                              | 62.04           | 21            | 158             | 21              |
| 67          | 26     | inc(4)   | 10               | 43                    | 11                | 47                     | 10                                | 43                              | 4.35            | 21            | 141             | 21              |
| 67          | 26     | sm(4)    | \-               | \-                    | 5                 | 36                     | \-                                | \-                              | 60.81           | 21            | 143             | 17              |
| 68          | 28     | inc(2)   | 7                | 23                    | 8                 | 25                     | 7                                 | 23                              | 0.73            | 21            | 70              | 15              |
| 68          | 28     | sm(2)    | \-               | \-                    | 8                 | 25                     | \-                                | \-                              | 62.82           | 21            | 110             | 16              |
| 68          | 28     | inc(3)   | 10               | 43                    | 13                | 58                     | 10                                | 43                              | 2.66            | 21            | 157             | 20              |
| 68          | 28     | sm(3)    | \-               | \-                    | 10                | 44                     | \-                                | \-                              | 80.96           | 21            | 195             | 20              |
| 68          | 28     | inc(4)   | 11               | 50                    | 14                | 68                     | 11                                | 50                              | 3.76            | 21            | 181             | 21              |
| 68          | 28     | sm(4)    | \-               | \-                    | 7                 | 47                     | \-                                | \-                              | 71.63           | 21            | 145             | 18              |
| 71          | 32     | inc(2)   | 7                | 25                    | 8                 | 27                     | 7                                 | 25                              | 0.98            | 24            | 81              | 16              |
| 71          | 32     | sm(2)    | \-               | \-                    | 9                 | 29                     | \-                                | \-                              | 55.46           | 24            | 83              | 16              |
| 71          | 32     | inc(3)   | 11               | 52                    | 12                | 58                     | 11                                | 52                              | 2.03            | 24            | 152             | 21              |
| 71          | 32     | sm(3)    | \-               | \-                    | 11                | 48                     | \-                                | \-                              | 63.97           | 24            | 194             | 20              |
| 71          | 32     | inc(4)   | 11               | 52                    | 13                | 68                     | 11                                | 52                              | 4.16            | 24            | 182             | 23              |
| 71          | 32     | sm(4)    | \-               | \-                    | 8                 | 51                     | \-                                | \-                              | 68.32           | 24            | 179             | 23              |
| 76          | 38     | inc(2)   | 8                | 27                    | 9                 | 29                     | 8                                 | 27                              | 0.55            | 26            | 77              | 18              |
| 76          | 38     | sm(2)    | \-               | \-                    | 10                | 31                     | \-                                | \-                              | 56.57           | 26            | 93              | 19              |
| 76          | 38     | inc(3)   | 13               | 60                    | 14                | 66                     | 13                                | 60                              | 2.25            | 26            | 155             | 23              |
| 76          | 38     | sm(3)    | \-               | \-                    | 13                | 52                     | \-                                | \-                              | 61.46           | 26            | 177             | 25              |
| 76          | 38     | inc(4)   | 13               | 59                    | 16                | 82                     | 13                                | 59                              | 4.28            | 26            | 205             | 26              |
| 76          | 38     | sm(4)    | \-               | \-                    | 11                | 66                     | \-                                | \-                              | 69.45           | 26            | 176             | 21              |
| 78          | 33     | inc(2)   | 6                | 21                    | 9                 | 32                     | 6                                 | 21                              | 2..55           | 31            | 112             | 24              |
| 78          | 33     | sm(2)    | \-               | \-                    | 9                 | 32                     | \-                                | \-                              | 57.63           | 31            | 116             | 24              |
| 78          | 33     | inc(3)   | 10               | 47                    | 16                | 85                     | 10                                | 47                              | 5.92            | 31            | 242             | 28              |
| 78          | 33     | sm(3)    | \-               | \-                    | 11                | 54                     | \-                                | \-                              | 64.24           | 31            | 219             | 30              |
| 78          | 33     | inc(4)   | 12               | 60                    | 21                | 121                    | 12                                | 60                              | 17.89           | 31            | 310             | 31              |
| 78          | 33     | sm(4)    | \-               | \-                    | 13                | 78                     | \-                                | \-                              | 65.74           | 31            | 232             | 30              |
| 83          | 35     | inc(2)   | 8                | 27                    | 11                | 38                     | 8                                 | 27                              | 3.01            | 34            | 127             | 23              |
| 83          | 35     | sm(2)    | \-               | \-                    | 12                | 40                     | \-                                | \-                              | 63.54           | 34            | 156             | 25              |
| 83          | 35     | inc(3)   | 13               | 60                    | 18                | 91                     | 13                                | 60                              | 7.32            | 34            | 254             | 30              |
| 83          | 35     | sm(3)    | \-               | \-                    | 14                | 62                     | \-                                | \-                              | 64.61           | 34            | 210             | 29              |
| 83          | 35     | inc(4)   | 14               | 66                    | 25                | 138                    | 14                                | 66                              | 20.66           | 34            | 327             | 33              |
| 83          | 35     | sm(4)    | \-               | \-                    | 14                | 82                     | \-                                | \-                              | 66.87           | 34            | 239             | 27              |
| 85          | 34     | inc(2)   | 9                | 32                    | 11                | 36                     | 9                                 | 32                              | 1.03            | 32            | 117             | 25              |
| 85          | 34     | sm(2)    | \-               | \-                    | 11                | 36                     | \-                                | \-                              | 58.66           | 32            | 141             | 25              |
| 85          | 34     | inc(3)   | 16               | 73                    | 18                | 77                     | 16                                | 73                              | 3.29            | 32            | 207             | 29              |
| 85          | 34     | sm(3)    | \-               | \-                    | 13                | 58                     | \-                                | \-                              | 63.23           | 32            | 240             | 31              |
| 85          | 34     | inc(4)   | 21               | 102                   | 23                | 106                    | 19                                | 86                              | 5.22            | 32            | 266             | 32              |
| 85          | 34     | sm(4)    | \-               | \-                    | 13                | 78                     | \-                                | \-                              | 63.83           | 32            | 237             | 29              |
| 86          | 39     | inc(2)   | 9                | 32                    | 10                | 34                     | 9                                 | 32                              | 0.86            | 33            | 124             | 23              |
| 86          | 39     | sm(2)    | \-               | \-                    | 10                | 34                     | \-                                | \-                              | 57.47           | 33            | 128             | 22              |
| 86          | 39     | inc(3)   | 15               | 66                    | 18                | 81                     | 15                                | 66                              | 2.41            | 33            | 232             | 31              |
| 86          | 39     | sm(3)    | \-               | \-                    | 13                | 58                     | \-                                | \-                              | 64.56           | 33            | 241             | 30              |
| 86          | 39     | inc(4)   | 20               | 95                    | 23                | 113                    | 18                                | 78                              | 4.49            | 33            | 278             | 32              |
| 86          | 39     | sm(4)    | \-               | \-                    | 16                | 93                     | \-                                | \-                              | 75.41           | 33            | 244             | 29              |
| 89          | 41     | inc(2)   | 11               | 38                    | 12                | 40                     | 11                                | 38                              | 0.66            | 37            | 110             | 22              |
| 89          | 41     | sm(2)    | \-               | \-                    | 13                | 42                     | \-                                | \-                              | 61.66           | 37            | 139             | 23              |
| 89          | 41     | inc(3)   | 17               | 72                    | 19                | 80                     | 17                                | 72                              | 2.70            | 37            | 199             | 29              |
| 89          | 41     | sm(3)    | \-               | \-                    | 16                | 66                     | \-                                | \-                              | 67.75           | 37            | 228             | 31              |
| 89          | 41     | inc(4)   | 22               | 101                   | 26                | 126                    | 19                                | 79                              | 4.02            | 37            | 297             | 35              |
| 89          | 41     | sm(4)    | \-               | \-                    | 17                | 97                     | \-                                | \-                              | 66.14           | 37            | 275             | 32              |

[Click for the PDF version of the table](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/Data%20on%20TestGeneration%26Execution.pdf)

## Reuse Rates
The table below shows reuse rates of test sequences and events in the testing scenarios.

| Scenario ID | Existing Product ID | PUC ID | Test Set | Test Sequences Reused in Test Set/PUC Number of Sequences | Test Sequences Reused in Test Set/Existing Product Number of Sequences | Events Reused in Test Sequences/PUC Number of Events | Events Reused in Test Sequences/Existing Product Number of Events |
| ----------- | ------------------- | ------ | -------- | --------------------------------------------------------- | ---------------------------------------------------------------------- | ---------------------------------------------------- | ----------------------------------------------------------------- |
| 2           | 0                   | 6      | inc(2)   | 75                                                        | 100                                                                    | 88.23529412                                          | 100                                                               |
| 2           | 0                   | 6      | inc(3)   | 71.42857143                                               | 100                                                                    | 71.11111111                                          | 100                                                               |
| 2           | 0                   | 6      | inc(4)   | 75                                                        | 100                                                                    | 70.90909091                                          | 100                                                               |
| 3           | 0                   | 24     | inc(2)   | 60                                                        | 100                                                                    | 78.94736842                                          | 100                                                               |
| 3           | 0                   | 24     | inc(3)   | 62.5                                                      | 100                                                                    | 74.41860465                                          | 100                                                               |
| 3           | 0                   | 24     | inc(4)   | 75                                                        | 100                                                                    | 90.69767442                                          | 100                                                               |
| 4           | 1                   | 2      | inc(2)   | 83.33333333                                               | 100                                                                    | 82.60869565                                          | 100                                                               |
| 4           | 1                   | 2      | inc(3)   | 88.88888889                                               | 100                                                                    | 90.69767442                                          | 100                                                               |
| 4           | 1                   | 2      | inc(4)   | 88.88888889                                               | 100                                                                    | 90.69767442                                          | 100                                                               |
| 5           | 1                   | 4      | inc(2)   | 83.33333333                                               | 100                                                                    | 90.47619048                                          | 100                                                               |
| 5           | 1                   | 4      | inc(3)   | 72.72727273                                               | 100                                                                    | 72.22222222                                          | 100                                                               |
| 5           | 1                   | 4      | inc(4)   | 66.66666667                                               | 100                                                                    | 60.9375                                              | 100                                                               |
| 17          | 5                   | 14     | inc(2)   | 85.71428571                                               | 100                                                                    | 92                                                   | 100                                                               |
| 17          | 5                   | 14     | inc(3)   | 83.33333333                                               | 100                                                                    | 79.03225806                                          | 100                                                               |
| 17          | 5                   | 14     | inc(4)   | 85.71428571                                               | 100                                                                    | 79.48717949                                          | 100                                                               |
| 19          | 6                   | 7      | inc(2)   | 66.66666667                                               | 100                                                                    | 80.95238095                                          | 100                                                               |
| 19          | 6                   | 7      | inc(3)   | 72.72727273                                               | 100                                                                    | 79.62962963                                          | 100                                                               |
| 19          | 6                   | 7      | inc(4)   | 83.33333333                                               | 100                                                                    | 93.33333333                                          | 100                                                               |
| 20          | 6                   | 9      | inc(2)   | 57.14285714                                               | 100                                                                    | 60.71428571                                          | 100                                                               |
| 20          | 6                   | 9      | inc(3)   | 57.14285714                                               | 100                                                                    | 53.08641975                                          | 100                                                               |
| 20          | 6                   | 9      | inc(4)   | 50                                                        | 100                                                                    | 44.44444444                                          | 100                                                               |
| 23          | 7                   | 8      | inc(2)   | 85.71428571                                               | 100                                                                    | 84                                                   | 100                                                               |
| 23          | 7                   | 8      | inc(3)   | 90.90909091                                               | 90.90909091                                                            | 105.8823529                                          | 100                                                               |
| 23          | 7                   | 8      | inc(4)   | 91.66666667                                               | 100                                                                    | 92.98245614                                          | 100                                                               |
| 31          | 9                   | 15     | inc(2)   | 87.5                                                      | 100                                                                    | 93.33333333                                          | 100                                                               |
| 31          | 9                   | 15     | inc(3)   | 81.25                                                     | 100                                                                    | 80.51948052                                          | 100                                                               |
| 31          | 9                   | 15     | inc(4)   | 85.71428571                                               | 100                                                                    | 83.48623853                                          | 100                                                               |
| 36          | 10                  | 19     | inc(2)   | 75                                                        | 100                                                                    | 74.41860465                                          | 100                                                               |
| 36          | 10                  | 19     | inc(3)   | 75                                                        | 100                                                                    | 73.33333333                                          | 100                                                               |
| 36          | 10                  | 19     | inc(4)   | 66.66666667                                               | 90                                                                     | 71.65354331                                          | 95.78947368                                                       |
| 39          | 11                  | 20     | inc(2)   | 75                                                        | 100                                                                    | 75.55555556                                          | 100                                                               |
| 39          | 11                  | 20     | inc(3)   | 80                                                        | 100                                                                    | 81.52173913                                          | 100                                                               |
| 39          | 11                  | 20     | inc(4)   | 67.85714286                                               | 90.47619048                                                            | 75.18796992                                          | 96.15384615                                                       |
| 41          | 12                  | 13     | inc(2)   | 71.42857143                                               | 100                                                                    | 82.60869565                                          | 100                                                               |
| 41          | 12                  | 13     | inc(3)   | 76.92307692                                               | 100                                                                    | 82.25806452                                          | 100                                                               |
| 41          | 12                  | 13     | inc(4)   | 86.66666667                                               | 100                                                                    | 94.59459459                                          | 100                                                               |
| 43          | 12                  | 36     | inc(2)   | 71.42857143                                               | 100                                                                    | 82.60869565                                          | 100                                                               |
| 43          | 12                  | 36     | inc(3)   | 76.92307692                                               | 100                                                                    | 82.25806452                                          | 100                                                               |
| 43          | 12                  | 36     | inc(4)   | 86.66666667                                               | 100                                                                    | 94.59459459                                          | 100                                                               |
| 49          | 15                  | 16     | inc(2)   | 80                                                        | 100                                                                    | 88.23529412                                          | 100                                                               |
| 49          | 15                  | 16     | inc(3)   | 88.88888889                                               | 100                                                                    | 95.0617284                                           | 100                                                               |
| 49          | 15                  | 16     | inc(4)   | 91.66666667                                               | 100                                                                    | 96.55172414                                          | 100                                                               |
| 50          | 15                  | 21     | inc(2)   | 72.72727273                                               | 100                                                                    | 73.17073171                                          | 100                                                               |
| 50          | 15                  | 21     | inc(3)   | 80                                                        | 100                                                                    | 81.91489362                                          | 100                                                               |
| 50          | 15                  | 21     | inc(4)   | 66.66666667                                               | 90.90909091                                                            | 68.75                                                | 98.21428571                                                       |
| 52          | 16                  | 17     | inc(2)   | 90.90909091                                               | 100                                                                    | 89.47368421                                          | 100                                                               |
| 52          | 16                  | 17     | inc(3)   | 89.47368421                                               | 100                                                                    | 87.05882353                                          | 100                                                               |
| 52          | 16                  | 17     | inc(4)   | 95.83333333                                               | 100                                                                    | 96.46017699                                          | 100                                                               |
| 54          | 16                  | 40     | inc(2)   | 83.33333333                                               | 100                                                                    | 89.47368421                                          | 100                                                               |
| 54          | 16                  | 40     | inc(3)   | 90                                                        | 100                                                                    | 95.29411765                                          | 100                                                               |
| 54          | 16                  | 40     | inc(4)   | 84.61538462                                               | 95.65217391                                                            | 89.16666667                                          | 96.3963964                                                        |
| 55          | 17                  | 23     | inc(2)   | 76.92307692                                               | 100                                                                    | 76.59574468                                          | 100                                                               |
| 55          | 17                  | 23     | inc(3)   | 81.81818182                                               | 100                                                                    | 83                                                   | 100                                                               |
| 55          | 17                  | 23     | inc(4)   | 70.96774194                                               | 95.65217391                                                            | 74.14965986                                          | 96.46017699                                                       |
| 62          | 21                  | 22     | inc(2)   | 83.33333333                                               | 100                                                                    | 90.47619048                                          | 100                                                               |
| 62          | 21                  | 22     | inc(3)   | 85.71428571                                               | 100                                                                    | 87.77777778                                          | 100                                                               |
| 62          | 21                  | 22     | inc(4)   | 88.88888889                                               | 92.30769231                                                            | 100                                                  | 99.21259843                                                       |
| 64          | 24                  | 25     | inc(2)   | 71.42857143                                               | 100                                                                    | 82.60869565                                          | 100                                                               |
| 64          | 24                  | 25     | inc(3)   | 81.81818182                                               | 100                                                                    | 92                                                   | 100                                                               |
| 64          | 24                  | 25     | inc(4)   | 81.81818182                                               | 100                                                                    | 92                                                   | 100                                                               |
| 66          | 24                  | 30     | inc(2)   | 83.33333333                                               | 100                                                                    | 90.47619048                                          | 100                                                               |
| 66          | 24                  | 30     | inc(3)   | 80                                                        | 100                                                                    | 75                                                   | 100                                                               |
| 66          | 24                  | 30     | inc(4)   | 81.81818182                                               | 100                                                                    | 74.19354839                                          | 100                                                               |
| 67          | 25                  | 26     | inc(2)   | 87.5                                                      | 100                                                                    | 85.18518519                                          | 100                                                               |
| 67          | 25                  | 26     | inc(3)   | 90.90909091                                               | 100                                                                    | 91.4893617                                           | 100                                                               |
| 67          | 25                  | 26     | inc(4)   | 90.90909091                                               | 100                                                                    | 91.4893617                                           | 100                                                               |
| 68          | 25                  | 28     | inc(2)   | 87.5                                                      | 100                                                                    | 92                                                   | 100                                                               |
| 68          | 25                  | 28     | inc(3)   | 76.92307692                                               | 100                                                                    | 74.13793103                                          | 100                                                               |
| 68          | 25                  | 28     | inc(4)   | 78.57142857                                               | 100                                                                    | 73.52941176                                          | 100                                                               |
| 71          | 26                  | 32     | inc(2)   | 87.5                                                      | 100                                                                    | 92.59259259                                          | 100                                                               |
| 71          | 26                  | 32     | inc(3)   | 91.66666667                                               | 100                                                                    | 89.65517241                                          | 100                                                               |
| 71          | 26                  | 32     | inc(4)   | 84.61538462                                               | 100                                                                    | 76.47058824                                          | 100                                                               |
| 76          | 29                  | 38     | inc(2)   | 88.88888889                                               | 100                                                                    | 93.10344828                                          | 100                                                               |
| 76          | 29                  | 38     | inc(3)   | 92.85714286                                               | 100                                                                    | 90.90909091                                          | 100                                                               |
| 76          | 29                  | 38     | inc(4)   | 81.25                                                     | 100                                                                    | 71.95121951                                          | 100                                                               |
| 78          | 30                  | 33     | inc(2)   | 66.66666667                                               | 100                                                                    | 65.625                                               | 100                                                               |
| 78          | 30                  | 33     | inc(3)   | 62.5                                                      | 100                                                                    | 55.29411765                                          | 100                                                               |
| 78          | 30                  | 33     | inc(4)   | 57.14285714                                               | 100                                                                    | 49.58677686                                          | 100                                                               |
| 83          | 32                  | 35     | inc(2)   | 72.72727273                                               | 100                                                                    | 71.05263158                                          | 100                                                               |
| 83          | 32                  | 35     | inc(3)   | 72.22222222                                               | 100                                                                    | 65.93406593                                          | 100                                                               |
| 83          | 32                  | 35     | inc(4)   | 56                                                        | 100                                                                    | 47.82608696                                          | 100                                                               |
| 85          | 33                  | 34     | inc(2)   | 81.81818182                                               | 100                                                                    | 88.88888889                                          | 100                                                               |
| 85          | 33                  | 34     | inc(3)   | 88.88888889                                               | 100                                                                    | 94.80519481                                          | 100                                                               |
| 85          | 33                  | 34     | inc(4)   | 82.60869565                                               | 90.47619048                                                            | 94.33962264                                          | 98.03921569                                                       |
| 86          | 33                  | 39     | inc(2)   | 90                                                        | 100                                                                    | 94.11764706                                          | 100                                                               |
| 86          | 33                  | 39     | inc(3)   | 83.33333333                                               | 100                                                                    | 81.48148148                                          | 100                                                               |
| 86          | 33                  | 39     | inc(4)   | 78.26086957                                               | 90                                                                     | 80.53097345                                          | 95.78947368                                                       |
| 89          | 35                  | 41     | inc(2)   | 91.66666667                                               | 100                                                                    | 95                                                   | 100                                                               |
| 89          | 35                  | 41     | inc(3)   | 89.47368421                                               | 100                                                                    | 90                                                   | 100                                                               |
| 89          | 35                  | 41     | inc(4)   | 73.07692308                                               | 86.36363636                                                            | 77.77777778                                          | 97.02970297                                                       |

[Click for the PDF version of the table](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccount/ReuseRates.pdf)
