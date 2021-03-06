# Student Attendance System

Student Attendance System product line has 20 features and a core feature. The core of the product line represents the common behavior which exists in all products that belong to Student Attendance System product line. The core behavior is modelled using core ESG (c-ESG). An optional behavior is modelled using a feature ESG (f-ESG). A featured ESG (FESG) is an extended ESG that is composed of a core ESG (c-ESG) and a set of feature ESGs (f-ESGs). A featured ESG is used in test sequence composition approach which composes the sequences of core and feature ESGs and generates a product's test sequences. The models of Student Attendance System product line are built from the users' perspective. The Event Sequence graphs' events are selected from user events.

## Feature Model

![Feature Model](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_ModelImages/StudentAttendanceSystemPL_featureModel.png)\
This feature model has 6 mandatory abstract features which means that at least or exactly one of their subfeatures has to be included in each product configuration. In this feature model various constraints are included such as the feature _edit schedule_ implies the feature _add new schedule_. 2664 different product configurations could be obtained by combining these features and applying the constraints of the feature model.

## Student Attendance System Products
There are 2664 product configurations in Student Attendance System Product Line. Due to the space concerns, we don't put all of the products' information here. In the table below, the product id and the belonging features are given. Since, each possible product does not have a unique official name, we assign IDs to products to name them uniquely.

| Product ID | Features                                                                                                                                                                                                              |
| ---------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1116       | viewClass, viewSchedule, email, studentAccess, teacherAccess, updateRecord, addNewClass, updateClassDetail, addNewSchedule, viewRecord, accessCard                                                                    |
| 210        | viewSchedule, SMS, studentAccess, teacherAccess, updateRecord, addNewClass, updateClassDetail, viewRecord, traceAttendanceActivity, fingerprint                                                                       |
| 2413       | viewClass, SMS, studentAccess, teacherAccess, updateRecord, addNewClass, updateClassDetail, addNewSchedule, editSchedule, deleteClass, assignNewSchedule, barcode                                                     |
| 2390       | viewClass, SMS, studentAccess, teacherAccess, updateRecord, addNewClass, updateClassDetail, addNewSchedule, editSchedule, traceAttendanceActivity, assignNewSchedule, fingerprint                                     |
| 1493       | viewClass, SMS, studentAccess, teacherAccess, updateRecord, addNewSchedule, editSchedule, monitorAttendanceStatus, barcode                                                                                            |
| 1803       | viewClass, viewSchedule, email, studentAccess, teacherAccess, addNewSchedule, editSchedule, viewRecord, monitorAttendanceStatus, QRCode                                                                               |
| 1231       | viewClass, viewSchedule, email, studentAccess, teacherAccess, addNewSchedule, viewRecord, monitorAttendanceStatus, deleteClass, QRCode                                                                                |
| 816        | viewClass, email, studentAccess, teacherAccess, updateRecord, addNewClass, addNewSchedule, monitorAttendanceStatus, deleteClass, accessCard                                                                           |
| 2655       | viewClass, viewSchedule, email, studentAccess, teacherAccess, updateRecord, addNewClass, updateClassDetail, addNewSchedule, editSchedule, viewRecord, traceAttendanceActivity, deleteClass, assignNewSchedule, QRCode |
| 2027       | viewClass, viewSchedule, email, studentAccess, teacherAccess, updateRecord, addNewClass, updateClassDetail, addNewSchedule, editSchedule, traceAttendanceActivity, QRCode                                             |
| 2211       | viewClass, viewSchedule, email, studentAccess, teacherAccess, updateRecord, addNewClass, addNewSchedule, editSchedule, viewRecord, deleteClass, QRCode                                                                |
| 2307       | viewClass, viewSchedule, email, teacherAccess, updateRecord, addNewClass, updateClassDetail, addNewSchedule, editSchedule, deleteClass, QRCode                                                                        |
| 2079       | viewSchedule, email, studentAccess, teacherAccess, updateRecord, addNewSchedule, editSchedule, traceAttendanceActivity, deleteClass, QRCode                                                                           |
| 1107       | viewClass, viewSchedule, email, studentAccess, teacherAccess, addNewClass, updateClassDetail, addNewSchedule, viewRecord, QRCode                                                                                      |
| 1412       | viewSchedule, email, studentAccess, teacherAccess, updateRecord, addNewClass, updateClassDetail, addNewSchedule, viewRecord, monitorAttendanceStatus, traceAttendanceActivity, deleteClass, accessCard                |
| 813        | viewClass, SMS, studentAccess, teacherAccess, addNewClass, addNewSchedule, viewRecord, monitorAttendanceStatus, deleteClass, barcode                                                                                  |
| 352        | viewClass, viewSchedule, email, studentAccess, teacherAccess, updateRecord, viewRecord, monitorAttendanceStatus, deleteClass, accessCard                                                                              |
| 1432       | viewClass, viewSchedule, email, studentAccess, teacherAccess, addNewClass, updateClassDetail, addNewSchedule, monitorAttendanceStatus, deleteClass, accessCard                                                        |
| 1562       | viewClass, SMS, studentAccess, teacherAccess, updateRecord, addNewClass, addNewSchedule, editSchedule, viewRecord, traceAttendanceActivity, fingerprint                                                               |
| 123        | viewClass, viewSchedule, email, teacherAccess, updateRecord, addNewClass, QRCode                                                                                                                                      |
| 1451       | viewClass, viewSchedule, email, teacherAccess, updateRecord, addNewClass, updateClassDetail, addNewSchedule, traceAttendanceActivity, deleteClass, QRCode                                                             |
| 1234       | viewClass, viewSchedule, SMS, studentAccess, teacherAccess, updateRecord, addNewSchedule, monitorAttendanceStatus, deleteClass, fingerprint                                                                           |
| 2328       | viewClass, viewSchedule, email, studentAccess, teacherAccess, updateRecord, addNewClass, updateClassDetail, addNewSchedule, editSchedule, viewRecord, monitorAttendanceStatus, deleteClass, accessCard                |
| 444        | viewClass, viewSchedule, email, studentAccess, teacherAccess, addNewClass, monitorAttendanceStatus, deleteClass, accessCard                                                                                           |
| 2183       | viewSchedule, email, studentAccess, teacherAccess, updateRecord, addNewClass, addNewSchedule, editSchedule, traceAttendanceActivity, deleteClass, QRCode                                                              |
| 487        | viewSchedule, email, teacherAccess, updateRecord, addNewClass, updateClassDetail, deleteClass, QRCode                                                                                                                 |
| 2279       | viewSchedule, email, studentAccess, teacherAccess, updateRecord, addNewClass, updateClassDetail, addNewSchedule, editSchedule, viewRecord, monitorAttendanceStatus, deleteClass, QRCode                               |
| 1634       | viewClass, SMS, studentAccess, teacherAccess, updateRecord, addNewSchedule, editSchedule, deleteClass, fingerprint                                                                                                    |
| 1246       | viewClass, viewSchedule, SMS, studentAccess, teacherAccess, updateRecord, addNewSchedule, traceAttendanceActivity, deleteClass, fingerprint                                                                           |
| 1005       | viewClass, viewSchedule, SMS, teacherAccess, updateRecord, addNewClass, addNewSchedule, barcode                                                                                                                       |

[Click for the PDF version of the table](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/Products.pdf)

# Student Attendance System Product Line Features
## Core ESG (c-ESG)
 ![core](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_ModelImages/core.PNG)\
 The core ESG of the Student Attendance System product line represents core features, which exist in all product configurations.\
 [Core ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_Models/core.zip)

## Student Access Feature ESG (f-ESG)
![studentAccess](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_ModelImages/studentAccess.PNG)\
Student Access feature enables the student user authorization.\
[Student Access Feature ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_Models/studentAccess.zip)

## Teacher Access Feature ESG (f-ESG)
![teacherAccess](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_ModelImages/teacherAccess.PNG)\
Teacher Access feature enables the teacher user authorization.\
[Teacher Access Feature ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_Models/teacherAccess.zip)

## Access Card Feature ESG (f-ESG)
![ccessCard](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_ModelImages/accessCard.PNG)\
Access Card feature enables the user authentication with an access card. \
[Access Card ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_Models/accessCard.zip)

## Barcode Feature ESG (f-ESG)
![barcode](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_ModelImages/barcode.PNG)\
Barcode feature enables the user authentication with a barcode. \
[Barcode ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_Models/barcode.zip)

## Fingerprint Feature ESG (f-ESG)
![fingerprint](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_ModelImages/fingerprint.PNG)\
Fingerprint feature enables the user authentication with his/her fingerprint. \
[Fingerprint ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_Models/fingerprint.zip)

## QR Code Feature ESG (f-ESG)
![QRCode](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_ModelImages/QRcode.PNG)\
QR code feature enables the user authentication with a QR code. \
[QR Code ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_Models/QRCode.zip)

## Email Feature ESG (f-ESG)
![email](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_ModelImages/email.PNG)\
Email feature enables the system to notify the user with email.\
[Email ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_Models/email.zip)

## SMS Feature ESG (f-ESG)
![SMS](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_ModelImages/SMS.PNG)\
SMS feature enables the system to notify the user with SMS.\
[SMS ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_Models/SMS.zip)

## View Record Feature ESG (f-ESG)
![viewRecord](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_ModelImages/viewRecord.PNG)\
View Record feature enables the user to select the existing attendance record and view it. \
[View Record ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_Models/viewRecord.zip)

## Update Record Feature ESG (f-ESG)
![updateRecord](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_ModelImages/updateRecord.PNG)\
Update Record feature enables the teacher user to select the existing attendace record and update it. \
[Update Record ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_Models/updateRecord.zip)

## Monitor Attendance Status Feature ESG (f-ESG)
![monitorAttendanceStatus](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_ModelImages/monitorAttendanceStatus.PNG)\
Monitor Attendance Status feature enables the student user to monitor the current attendace status.\
[Monitor Attendance Status ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_Models/monitorAttendanceStatus.zip)

## Trace Attendance Activity Feature ESG (f-ESG)
![traceAttendanceActivity](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_ModelImages/traceAttendanceActivity.PNG)\
Trace Attendance Activity feature enables the user to trace the attendance activity of a class.\
[Trace Attendance Activity ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_Models/traceAttendanceActivity.zip)

## View Class Feature ESG (f-ESG)
![viewClass](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_ModelImages/viewClass.PNG)\
View Class feature enables the user to select the existing class record and view it.\
[View Class ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_Models/viewClass.zip)

## Add New Class Feature ESG (f-ESG)
![addNewClass](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_ModelImages/addNewClass.PNG)\
Add New Class feature enables the teacher to add new class.\
[Add New Class ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_Models/addNewClass.zip)

## Update Class Detail Feature ESG (f-ESG)
![updateClassDetail](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_ModelImages/updateClassDetail.PNG)\
Update Class Detail feature enables the teacher user to update a class' detail.\
[Update Class Detail ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_Models/updateClassDetail.zip)

## Delete Class Activity Feature ESG (f-ESG)
![deleteClass](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_ModelImages/deleteClass.PNG)\
Delete Class feature enables the teacher user to delete a class.\
[Delete Class ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_Models/deleteClass.zip)

## View Schedule Feature ESG (f-ESG)
![viewSchedule](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_ModelImages/viewSchedule.PNG)\
View Schedule feature enables the user to view the schedule of a class.\
[View Schedule ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_Models/viewSchedule.zip)

## Add New Schedule Feature ESG (f-ESG)
![addNewSchedule](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_ModelImages/addNewSchedule.PNG)\
Add New Schedule feature enables the teacher user to add a new schedule to a class. \
[Add New Schedule ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_Models/addNewSchedule.zip)

## Edit Scheudule Feature ESG (f-ESG)
![editScheudule](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_ModelImages/editSchedule.PNG)\
Edit Scheudule feature enables the teacher user to edit the schedule of a class.\
[Edit Scheudule ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_Models/editSchedule.zip)

## Assign New Schedule Feature ESG (f-ESG)
![assignNewSchedule](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_ModelImages/assignNewSchedule.PNG)\
Assign New Schedule feature enables the teacher user to assign a a new schedule to a class.\
[Assign New Schedule ESG MXE File](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_Models/assignNewSchedule.zip)

# Student Attendance System Product Line Test Generation and Execution
The Student Attendance System product line has 2664 product configurations and 10236 one-increment, i.e., one feature addition, testing scenarios in total. In our study, we select 30 of the testing scenarios randomly. In the selection process of the one increment scenarios, the following two rules are applied:
1.	The same scenario has not been selected more than once.	
2.	The same PUC has not been selected more than twice.

## Testing Scenarios
In this table, the selected testing scenarios are given with their Scenario IDs, Product Under Consideration(PUC) IDs, Existing Product IDs and Features and Increment. Existing Product refers to the product that we already have the model and the test sequences. In incremental test generation approach, the existing product's test sequences and increment's test sequences are composed so that the test sequences of the PUC is obtained without generating and composing all of its features from scratch. 

| Scenario ID | Product Under Consideration ID | Existing Product ID | EP Features                                                                                                                                                                                        | New Feature               |
| ----------- | ------------------------------ | ------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------- |
| 4852        | 1116                           | 1112                | viewClass, viewSchedule, email, studentAccess, teacherAccess, updateRecord, addNewClass, updateClassDetail, addNewSchedule, accessCard                                                             | viewRecord              |
| 962         | 210                            | 206                 | viewSchedule, SMS, studentAccess, teacherAccess, updateRecord, addNewClass, updateClassDetail, traceAttendanceActivity, fingerprint                                                                | viewRecord              |
| 9432        | 2413                           | 2361                | viewClass, SMS, studentAccess, teacherAccess, updateRecord, addNewClass, updateClassDetail, addNewSchedule, editSchedule, assignNewSchedule, barcode                                               | deleteClass             |
| 9436        | 2390                           | 2362                | viewClass, SMS, studentAccess, teacherAccess, updateRecord, addNewClass, updateClassDetail, addNewSchedule, editSchedule, assignNewSchedule, fingerprint                                           | traceAttendanceActivity |
| 2511        | 1493                           | 609                 | viewClass, SMS, studentAccess, teacherAccess, updateRecord, addNewSchedule, monitorAttendanceStatus, barcode                                                                                       | editSchedule            |
| 7500        | 1803                           | 1799                | viewClass, viewSchedule, email, studentAccess, teacherAccess, addNewSchedule, editSchedule, monitorAttendanceStatus, QRCode                                                                        | viewRecord              |
| 3942        | 1231                           | 919                 | viewClass, viewSchedule, email, studentAccess, teacherAccess, addNewSchedule, viewRecord, monitorAttendanceStatus, QRCode                                                                          | deleteClass             |
| 3445        | 816                            | 800                 | viewClass, email, studentAccess, teacherAccess, updateRecord, addNewClass, addNewSchedule, deleteClass, accessCard                                                                                 | monitorAttendanceStatus |
| 9379        | 2655                           | 2343                | viewClass, viewSchedule, email, studentAccess, teacherAccess, updateRecord, addNewClass, updateClassDetail, addNewSchedule, editSchedule, viewRecord, traceAttendanceActivity, deleteClass, QRCode | assignNewSchedule       |
| 4971        | 2027                           | 1143                | viewClass, viewSchedule, email, studentAccess, teacherAccess, updateRecord, addNewClass, updateClassDetail, addNewSchedule, traceAttendanceActivity, QRCode                                        | editSchedule            |
| 7119        | 2211                           | 1691                | viewClass, email, studentAccess, teacherAccess, updateRecord, addNewClass, addNewSchedule, editSchedule, viewRecord, deleteClass, QRCode                                                           | viewSchedule            |
| 6051        | 2307                           | 1423                | viewClass, viewSchedule, email, teacherAccess, updateRecord, addNewClass, updateClassDetail, addNewSchedule, deleteClass, QRCode                                                                   | editSchedule            |
| 8577        | 2079                           | 2127                | viewSchedule, email, teacherAccess, updateRecord, addNewSchedule, editSchedule, traceAttendanceActivity, deleteClass, QRCode                                                                       | studentAccess           |
| 4365        | 1107                           | 1003                | viewClass, viewSchedule, email, studentAccess, teacherAccess, addNewClass, addNewSchedule, viewRecord, QRCode                                                                                      | updateClassDetail       |
| 2217        | 1412                           | 528                 | viewSchedule, email, studentAccess, teacherAccess, updateRecord, addNewClass, updateClassDetail, viewRecord, monitorAttendanceStatus, traceAttendanceActivity, deleteClass, accessCard             | addNewSchedule          |
| 3493        | 813                            | 809                 | viewClass, SMS, studentAccess, teacherAccess, addNewClass, addNewSchedule, monitorAttendanceStatus, deleteClass, barcode                                                                           | viewRecord              |
| 1341        | 352                            | 300                 | viewSchedule, email, studentAccess, teacherAccess, updateRecord, viewRecord, monitorAttendanceStatus, deleteClass, accessCard                                                                      | viewClass               |
| 5914        | 1432                           | 1380                | viewSchedule, email, studentAccess, teacherAccess, addNewClass, updateClassDetail, addNewSchedule, monitorAttendanceStatus, deleteClass, accessCard                                                | viewClass               |
| 6361        | 1562                           | 1510                | viewClass, SMS, studentAccess, teacherAccess, updateRecord, addNewSchedule, editSchedule, viewRecord, traceAttendanceActivity, fingerprint                                                         | addNewClass             |
| 45          | 123                            | 11                  | viewClass, viewSchedule, email, teacherAccess, updateRecord, QRCode                                                                                                                                | addNewClass             |
| 6050        | 1451                           | 1423                | viewClass, viewSchedule, email, teacherAccess, updateRecord, addNewClass, updateClassDetail, addNewSchedule, deleteClass, QRCode                                                                   | traceAttendanceActivity |
| 5283        | 1234                           | 1218                | viewClass, viewSchedule, SMS, studentAccess, teacherAccess, updateRecord, addNewSchedule, deleteClass, fingerprint                                                                                 | monitorAttendanceStatus |
| 7349        | 2328                           | 1756                | viewClass, email, studentAccess, teacherAccess, updateRecord, addNewClass, updateClassDetail, addNewSchedule, editSchedule, viewRecord, monitorAttendanceStatus, deleteClass, accessCard           | viewSchedule            |
| 1706        | 444                            | 392                 | viewSchedule, email, studentAccess, teacherAccess, addNewClass, monitorAttendanceStatus, deleteClass, accessCard                                                                                   | viewClass               |
| 5615        | 2183                           | 1299                | viewSchedule, email, studentAccess, teacherAccess, updateRecord, addNewClass, addNewSchedule, traceAttendanceActivity, deleteClass, QRCode                                                         | editSchedule            |
| 1658        | 487                            | 383                 | viewSchedule, email, teacherAccess, updateRecord, addNewClass, deleteClass, QRCode                                                                                                                 | updateClassDetail       |
| 8178        | 2279                           | 1967                | viewSchedule, email, studentAccess, teacherAccess, updateRecord, addNewClass, updateClassDetail, addNewSchedule, editSchedule, viewRecord, monitorAttendanceStatus, QRCode                         | deleteClass             |
| 3225        | 1634                           | 750                 | viewClass, SMS, studentAccess, teacherAccess, updateRecord, addNewSchedule, deleteClass, fingerprint                                                                                               | editSchedule            |
| 5188        | 1246                           | 1194                | viewSchedule, SMS, studentAccess, teacherAccess, updateRecord, addNewSchedule, traceAttendanceActivity, deleteClass, fingerprint                                                                   | viewClass               |
| 573         | 1005                           | 121                 | viewClass, viewSchedule, SMS, teacherAccess, updateRecord, addNewClass, barcode                                                                                                                    | addNewSchedule          |

[Click for the PDF version of the table](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/TestingScenarios.pdf)

## Data on PUCs
The numbers of k-sequences where k=1,2,3,4 are given to give a notion of the sizes of the selected PUCs in the testing scenarios.

| Product Under Consideration ID | k = 1 |  k = 2 | k = 3 | k = 4 |
| ------------------------------ | ----- | ------ | ----- | ----- |
| 1116                           | 34    | 53     | 94    | 168   |
| 210                            | 29    | 43     | 69    | 116   |
| 2413                           | 38    | 68     | 124   | 232   |
| 2390                           | 35    | 62     | 116   | 223   |
| 1493                           | 28    | 44     | 71    | 118   |
| 1803                           | 27    | 40     | 68    | 118   |
| 1231                           | 27    | 35     | 52    | 79    |
| 816                            | 31    | 45     | 72    | 120   |
| 2655                           | 42    | 70     | 128   | 239   |
| 2027                           | 36    | 61     | 114   | 212   |
| 2211                           | 37    | 57     | 99    | 174   |
| 2307                           | 36    | 60     | 111   | 208   |
| 2079                           | 30    | 45     | 72    | 120   |
| 1107                           | 30    | 48     | 88    | 162   |
| 1412                           | 37    | 57     | 96    | 168   |
| 813                            | 30    | 45     | 72    | 120   |
| 352                            | 27    | 31     | 37    | 40    |
| 1432                           | 32    | 51     | 92    | 167   |
| 1562                           | 33    | 52     | 90    | 161   |
| 123                            | 23    | 29     | 43    | 67    |
| 1451                           | 34    | 52     | 91    | 164   |
| 1234                           | 29    | 38     | 56    | 83    |
| 2328                           | 41    | 67     | 121   | 220   |
| 444                            | 25    | 33     | 50    | 77    |
| 2183                           | 34    | 54     | 93    | 165   |
| 487                            | 27    | 40     | 66    | 114   |
| 2279                           | 39    | 65     | 116   | 212   |
| 1634                           | 29    | 44     | 71    | 119   |
| 1246                           | 29    | 38     | 56    | 83    |
| 1005                           | 28    | 41     | 68    | 116   |

[Click for the PDF version of the table](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/Data%20on%20PUCs.pdf)

## Data on Number of Faults
The table below contains the total number of possible faults and the number of faults seeded for various m values for each PUC. The entire number of possible faults for each PUC for a given value of m is directly proportional to the number of m-sequences in the PUC's ESG, and the total number of seeded faults is 20% of the summation of number of possible faults for m=2,3,4,5.

| Scenario ID | PUC ID | m=2 | m=3 | m=4 | m=5 | Total Number of Possible Faults | Number of Seeded Faults |
| ----------- | ------ | --- | --- | --- | --- | ----------------------------- | ----------------------- |
| 45          | 123    | 52  | 72  | 110 | 178 | 412                           | 82                      |
| 573         | 1005   | 69  | 109 | 184 | 323 | 685                           | 137                     |
| 962         | 210    | 72  | 112 | 185 | 320 | 689                           | 138                     |
| 1341        | 352    | 58  | 68  | 77  | 72  | 275                           | 55                      |
| 1658        | 487    | 67  | 106 | 180 | 319 | 672                           | 134                     |
| 1706        | 444    | 58  | 83  | 127 | 194 | 462                           | 92                      |
| 2217        | 1412   | 94  | 153 | 264 | 470 | 981                           | 196                     |
| 2511        | 1493   | 72  | 115 | 189 | 324 | 700                           | 140                     |
| 3225        | 1634   | 73  | 115 | 190 | 327 | 705                           | 141                     |
| 3445        | 816    | 76  | 117 | 192 | 328 | 713                           | 143                     |
| 3493        | 813    | 75  | 117 | 192 | 327 | 711                           | 142                     |
| 3942        | 1231   | 62  | 87  | 131 | 197 | 477                           | 95                      |
| 4365        | 1107   | 78  | 136 | 250 | 458 | 922                           | 184                     |
| 4852        | 1116   | 87  | 147 | 262 | 470 | 966                           | 193                     |
| 4971        | 2027   | 97  | 175 | 326 | 606 | 1204                          | 241                     |
| 5188        | 1246   | 67  | 94  | 139 | 207 | 507                           | 101                     |
| 5283        | 1234   | 67  | 94  | 139 | 206 | 506                           | 101                     |
| 5615        | 2183   | 88  | 147 | 258 | 466 | 959                           | 192                     |
| 5914        | 1432   | 83  | 143 | 259 | 468 | 953                           | 191                     |
| 6050        | 1451   | 86  | 143 | 255 | 466 | 950                           | 190                     |
| 6051        | 2307   | 96  | 171 | 319 | 601 | 1187                          | 237                     |
| 6361        | 1562   | 85  | 142 | 251 | 457 | 935                           | 187                     |
| 7119        | 2211   | 94  | 156 | 273 | 482 | 1005                          | 201                     |
| 7349        | 2328   | 108 | 188 | 341 | 620 | 1257                          | 251                     |
| 7500        | 1803   | 67  | 108 | 186 | 322 | 683                           | 137                     |
| 8178        | 2279   | 104 | 181 | 328 | 605 | 1218                          | 244                     |
| 8577        | 2079   | 75  | 117 | 192 | 329 | 713                           | 143                     |
| 9379        | 2655   | 112 | 198 | 367 | 683 | 1360                          | 272                     |
| 9432        | 2413   | 106 | 192 | 356 | 671 | 1325                          | 265                     |
| 9436        | 2390   | 97  | 178 | 339 | 653 | 1267                          | 253                     |

[Click for the PDF version of the table](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/Data%20on%20Number%20of%20Faults.pdf)

## Data on Test Generation and Execution
Table below presents data on fault coverage and performance statistics on test set generation and test execution processes.

| Scenario ID | PUC ID | Test Set | EP Test Set Size | Length of EP Test Set | PUC Test Set Size | Length of PUC Test Set | Test Sequences Reused in Test Set | Events Reused in Test Sequences | Generation Time | Faults Seeded | Events Executed | Faults Revealed |
| ----------- | ------ | -------- | ---------------- | --------------------- | ----------------- | ---------------------- | --------------------------------- | ------------------------------- | --------------- | ------------- | --------------- | --------------- |
| 45          | 1.23   | inc(2)   | 6                | 35                    | 8                 | 51                     | 6                                 | 35                              | 1.23            | 82            | 307             | 52              |
| 45          | 123    | sm(2)    | \-               | \-                    | 8                 | 51                     | \-                                | \-                              | 64.35           | 82            | 298             | 51              |
| 45          | 123    | inc(3)   | 9                | 52                    | 15                | 100                    | 9                                 | 52                              | 3.44            | 82            | 453             | 66              |
| 45          | 123    | sm(3)    | \-               | \-                    | 15                | 100                    | \-                                | \-                              | 68.45           | 82            | 464             | 66              |
| 45          | 123    | inc(4)   | 10               | 57                    | 24                | 177                    | 10                                | 57                              | 12.83           | 82            | 583             | 72              |
| 45          | 123    | sm(4)    | \-               | \-                    | 24                | 177                    | \-                                | \-                              | 86.54           | 82            | 577             | 71              |
| 573         | 1.26   | inc(2)   | 10               | 58                    | 12                | 74                     | 10                                | 58                              | 1.26            | 137           | 523             | 87              |
| 573         | 1005   | sm(2)    | \-               | \-                    | 12                | 74                     | \-                                | \-                              | 62.79           | 137           | 544             | 90              |
| 573         | 1005   | inc(3)   | 18               | 112                   | 24                | 160                    | 18                                | 112                             | 4.25            | 137           | 780             | 109             |
| 573         | 1005   | sm(3)    | \-               | \-                    | 24                | 160                    | \-                                | \-                              | 106.03          | 137           | 772             | 109             |
| 573         | 1005   | inc(4)   | 28               | 195                   | 42                | 315                    | 24                                | 155                             | 18.20           | 137           | 1079            | 127             |
| 573         | 1005   | sm(4)    | \-               | \-                    | 42                | 315                    | \-                                | \-                              | 119.09          | 137           | 1095            | 128             |
| 962         | 0.9    | inc(2)   | 13               | 84                    | 14                | 89                     | 13                                | 84                              | 0.90            | 138           | 489             | 80              |
| 962         | 210    | sm(2)    | \-               | \-                    | 14                | 89                     | \-                                | \-                              | 69.07           | 138           | 490             | 80              |
| 962         | 210    | inc(3)   | 22               | 152                   | 23                | 157                    | 22                                | 152                             | 1.65            | 138           | 751             | 107             |
| 962         | 210    | sm(3)    | \-               | \-                    | 23                | 157                    | \-                                | \-                              | 83.96           | 138           | 748             | 107             |
| 962         | 210    | inc(4)   | 39               | 301                   | 40                | 306                    | 31                                | 221                             | 7.62            | 138           | 1122            | 129             |
| 962         | 210    | sm(4)    | \-               | \-                    | 40                | 306                    | \-                                | \-                              | 114.08          | 138           | 1106            | 128             |
| 1341        | 0.85   | inc(2)   | 11               | 64                    | 12                | 69                     | 11                                | 64                              | 0.85            | 55            | 274             | 46              |
| 1341        | 352    | sm(2)    | \-               | \-                    | 11                | 64                     | \-                                | \-                              | 78.28           | 55            | 263             | 44              |
| 1341        | 352    | inc(3)   | 12               | 68                    | 16                | 92                     | 12                                | 68                              | 2.93            | 55            | 330             | 52              |
| 1341        | 352    | sm(3)    | \-               | \-                    | 16                | 92                     | \-                                | \-                              | 72.56           | 55            | 331             | 52              |
| 1341        | 352    | inc(4)   | 14               | 79                    | 18                | 103                    | 14                                | 79                              | 7.63            | 55            | 356             | 55              |
| 1341        | 352    | sm(4)    | \-               | \-                    | 17                | 97                     | \-                                | \-                              | 79.13           | 55            | 351             | 55              |
| 1658        | 1.6    | inc(2)   | 9                | 60                    | 11                | 76                     | 9                                 | 60                              | 1.60            | 134           | 518             | 84              |
| 1658        | 487    | sm(2)    | \-               | \-                    | 11                | 76                     | \-                                | \-                              | 62.37           | 134           | 516             | 84              |
| 1658        | 487    | inc(3)   | 14               | 96                    | 21                | 150                    | 14                                | 96                              | 3.71            | 134           | 744             | 105             |
| 1658        | 487    | sm(3)    | \-               | \-                    | 20                | 144                    | \-                                | \-                              | 119.83          | 134           | 734             | 105             |
| 1658        | 487    | inc(4)   | 24               | 179                   | 38                | 299                    | 21                                | 148                             | 19.67           | 134           | 1074            | 123             |
| 1658        | 487    | sm(4)    | \-               | \-                    | 37                | 293                    | \-                                | \-                              | 162.22          | 134           | 1071            | 124             |
| 1706        | 0.76   | inc(2)   | 10               | 61                    | 11                | 66                     | 10                                | 61                              | 0.76            | 92            | 350             | 61              |
| 1706        | 444    | sm(2)    | \-               | \-                    | 10                | 61                     | \-                                | \-                              | 64.53           | 92            | 360             | 62              |
| 1706        | 444    | inc(3)   | 15               | 97                    | 19                | 121                    | 15                                | 97                              | 2.81            | 92            | 512             | 75              |
| 1706        | 444    | sm(3)    | \-               | \-                    | 19                | 121                    | \-                                | \-                              | 72.20           | 92            | 514             | 75              |
| 1706        | 444    | inc(4)   | 25               | 180                   | 29                | 204                    | 23                                | 157                             | 5.24            | 92            | 698             | 87              |
| 1706        | 444    | sm(4)    | \-               | \-                    | 28                | 198                    | \-                                | \-                              | 112.25          | 92            | 703             | 87              |
| 2217        | 1.38   | inc(2)   | 16               | 102                   | 18                | 118                    | 16                                | 102                             | 1.38            | 196           | 779             | 124             |
| 2217        | 1412   | sm(2)    | \-               | \-                    | 18                | 118                    | \-                                | \-                              | 71.05           | 196           | 777             | 124             |
| 2217        | 1412   | inc(3)   | 25               | 170                   | 32                | 224                    | 25                                | 170                             | 4.18            | 196           | 1117            | 154             |
| 2217        | 1412   | sm(3)    | \-               | \-                    | 31                | 218                    | \-                                | \-                              | 112.86          | 196           | 1113            | 154             |
| 2217        | 1412   | inc(4)   | 43               | 325                   | 57                | 445                    | 39                                | 282                             | 13.07           | 196           | 1602            | 179             |
| 2217        | 1412   | sm(4)    | \-               | \-                    | 56                | 439                    | \-                                | \-                              | 150.16          | 196           | 1569            | 178             |
| 2511        | 1.51   | inc(2)   | 13               | 73                    | 15                | 89                     | 13                                | 73                              | 1.51            | 140           | 515             | 86              |
| 2511        | 1493   | sm(2)    | \-               | \-                    | 15                | 89                     | \-                                | \-                              | 90.68           | 140           | 513             | 86              |
| 2511        | 1493   | inc(3)   | 19               | 114                   | 25                | 162                    | 19                                | 114                             | 4.78            | 140           | 776             | 113             |
| 2511        | 1493   | sm(3)    | \-               | \-                    | 25                | 162                    | \-                                | \-                              | 92.66           | 140           | 781             | 113             |
| 2511        | 1493   | inc(4)   | 29               | 197                   | 43                | 317                    | 25                                | 157                             | 23.40           | 140           | 1097            | 130             |
| 2511        | 1493   | sm(4)    | \-               | \-                    | 43                | 317                    | \-                                | \-                              | 125.63          | 140           | 1081            | 130             |
| 3225        | 1.3    | inc(2)   | 11               | 71                    | 13                | 87                     | 11                                | 71                              | 1.30            | 141           | 527             | 88              |
| 3225        | 1634   | sm(2)    | \-               | \-                    | 13                | 87                     | \-                                | \-                              | 99.82           | 141           | 527             | 88              |
| 3225        | 1634   | inc(3)   | 16               | 107                   | 23                | 161                    | 16                                | 107                             | 4.24            | 141           | 764             | 109             |
| 3225        | 1634   | sm(3)    | \-               | \-                    | 22                | 155                    | \-                                | \-                              | 86.07           | 141           | 753             | 109             |
| 3225        | 1634   | inc(4)   | 26               | 190                   | 40                | 310                    | 24                                | 169                             | 33.87           | 141           | 1099            | 131             |
| 3225        | 1634   | sm(4)    | \-               | \-                    | 39                | 304                    | \-                                | \-                              | 115.59          | 141           | 1101            | 130             |
| 3445        | 0.83   | inc(2)   | 13               | 87                    | 14                | 91                     | 13                                | 87                              | 0.83            | 143           | 537             | 90              |
| 3445        | 816    | sm(2)    | \-               | \-                    | 14                | 91                     | \-                                | \-                              | 83.51           | 143           | 541             | 90              |
| 3445        | 816    | inc(3)   | 22               | 155                   | 23                | 159                    | 22                                | 155                             | 1.61            | 143           | 785             | 114             |
| 3445        | 816    | sm(3)    | \-               | \-                    | 23                | 159                    | \-                                | \-                              | 84.27           | 143           | 792             | 114             |
| 3445        | 816    | inc(4)   | 40               | 310                   | 41                | 314                    | 34                                | 250                             | 4.16            | 143           | 1136            | 134             |
| 3445        | 816    | sm(4)    | \-               | \-                    | 40                | 308                    | \-                                | \-                              | 111.66          | 143           | 1142            | 135             |
| 3493        | 1.05   | inc(2)   | 14               | 84                    | 15                | 89                     | 14                                | 84                              | 1.05            | 142           | 509             | 92              |
| 3493        | 813    | sm(2)    | \-               | \-                    | 15                | 89                     | \-                                | \-                              | 67.18           | 142           | 513             | 92              |
| 3493        | 813    | inc(3)   | 24               | 157                   | 25                | 162                    | 24                                | 157                             | 2.12            | 142           | 747             | 113             |
| 3493        | 813    | sm(3)    | \-               | \-                    | 25                | 162                    | \-                                | \-                              | 109.80          | 142           | 746             | 113             |
| 3493        | 813    | inc(4)   | 43               | 318                   | 44                | 323                    | 37                                | 257                             | 4.24            | 142           | 1093            | 131             |
| 3493        | 813    | sm(4)    | \-               | \-                    | 43                | 317                    | \-                                | \-                              | 124.00          | 142           | 1078            | 131             |
| 3942        | 1.3    | inc(2)   | 10               | 57                    | 11                | 66                     | 10                                | 57                              | 1.30            | 95            | 363             | 61              |
| 3942        | 1231   | sm(2)    | \-               | \-                    | 11                | 66                     | \-                                | \-                              | 67.52           | 95            | 389             | 64              |
| 3942        | 1231   | inc(3)   | 19               | 117                   | 20                | 126                    | 19                                | 117                             | 3.94            | 95            | 537             | 81              |
| 3942        | 1231   | sm(3)    | \-               | \-                    | 20                | 126                    | \-                                | \-                              | 116.56          | 95            | 537             | 81              |
| 3942        | 1231   | inc(4)   | 28               | 194                   | 30                | 209                    | 24                                | 154                             | 7.50            | 95            | 716             | 90              |
| 3942        | 1231   | sm(4)    | \-               | \-                    | 29                | 203                    | \-                                | \-                              | 151.83          | 95            | 715             | 90              |
| 4365        | 1.29   | inc(2)   | 11               | 69                    | 13                | 85                     | 11                                | 69                              | 1.29            | 184           | 592             | 99              |
| 4365        | 1107   | sm(2)    | \-               | \-                    | 13                | 85                     | \-                                | \-                              | 64.69           | 184           | 605             | 101             |
| 4365        | 1107   | inc(3)   | 24               | 161                   | 30                | 209                    | 24                                | 161                             | 4.83            | 184           | 951             | 132             |
| 4365        | 1107   | sm(3)    | \-               | \-                    | 30                | 209                    | \-                                | \-                              | 92.32           | 184           | 958             | 132             |
| 4365        | 1107   | inc(4)   | 41               | 310                   | 55                | 430                    | 35                                | 249                             | 13.15           | 184           | 1486            | 164             |
| 4365        | 1107   | sm(4)    | \-               | \-                    | 55                | 430                    | \-                                | \-                              | 135.49          | 184           | 1467            | 163             |
| 4852        | 0.77   | inc(2)   | 14               | 94                    | 15                | 99                     | 14                                | 94                              | 0.77            | 193           | 669             | 112             |
| 4852        | 1116   | sm(2)    | \-               | \-                    | 15                | 99                     | \-                                | \-                              | 76.57           | 193           | 647             | 108             |
| 4852        | 1116   | inc(3)   | 31               | 218                   | 32                | 223                    | 31                                | 218                             | 2.17            | 193           | 1045            | 146             |
| 4852        | 1116   | sm(3)    | \-               | \-                    | 32                | 223                    | \-                                | \-                              | 127.28          | 193           | 1038            | 146             |
| 4852        | 1116   | inc(4)   | 56               | 439                   | 57                | 444                    | 46                                | 338                             | 3.59            | 193           | 1582            | 179             |
| 4852        | 1116   | sm(4)    | \-               | \-                    | 57                | 444                    | \-                                | \-                              | 141.90          | 193           | 1552            | 178             |
| 4971        | 1.59   | inc(2)   | 15               | 100                   | 17                | 116                    | 15                                | 100                             | 1.59            | 241           | 878             | 140             |
| 4971        | 2027   | sm(2)    | \-               | \-                    | 17                | 116                    | \-                                | \-                              | 69.00           | 241           | 867             | 138             |
| 4971        | 2027   | inc(3)   | 32               | 224                   | 38                | 272                    | 32                                | 224                             | 5.98            | 241           | 1345            | 186             |
| 4971        | 2027   | sm(3)    | \-               | \-                    | 38                | 272                    | \-                                | \-                              | 122.20          | 241           | 1352            | 186             |
| 4971        | 2027   | inc(4)   | 57               | 445                   | 71                | 565                    | 50                                | 371                             | 16.22           | 241           | 1985            | 219             |
| 4971        | 2027   | sm(4)    | \-               | \-                    | 71                | 565                    | \-                                | \-                              | 240.16          | 241           | 1985            | 220             |
| 5188        | 1.29   | inc(2)   | 12               | 77                    | 13                | 82                     | 12                                | 77                              | 1.29            | 101           | 371             | 62              |
| 5188        | 1246   | sm(2)    | \-               | \-                    | 12                | 77                     | \-                                | \-                              | 65.63           | 101           | 368             | 61              |
| 5188        | 1246   | inc(3)   | 17               | 113                   | 21                | 137                    | 17                                | 113                             | 3.33            | 101           | 570             | 82              |
| 5188        | 1246   | sm(3)    | \-               | \-                    | 21                | 137                    | \-                                | \-                              | 101.26          | 101           | 567             | 82              |
| 5188        | 1246   | inc(4)   | 27               | 196                   | 31                | 220                    | 24                                | 165                             | 6.48            | 101           | 771             | 94              |
| 5188        | 1246   | sm(4)    | \-               | \-                    | 30                | 214                    | \-                                | \-                              | 100.65          | 101           | 783             | 96              |
| 5283        | 0.7    | inc(2)   | 11               | 71                    | 12                | 75                     | 11                                | 71                              | 0.70            | 101           | 379             | 63              |
| 5283        | 1234   | sm(2)    | \-               | \-                    | 12                | 75                     | \-                                | \-                              | 68.41           | 101           | 364             | 60              |
| 5283        | 1234   | inc(3)   | 20               | 131                   | 21                | 135                    | 20                                | 131                             | 2.05            | 101           | 584             | 84              |
| 5283        | 1234   | sm(3)    | \-               | \-                    | 21                | 135                    | \-                                | \-                              | 81.63           | 101           | 589             | 84              |
| 5283        | 1234   | inc(4)   | 30               | 214                   | 31                | 218                    | 26                                | 174                             | 3.41            | 101           | 783             | 96              |
| 5283        | 1234   | sm(4)    | \-               | \-                    | 30                | 212                    | \-                                | \-                              | 113.80          | 101           | 771             | 97              |
| 5615        | 1.27   | inc(2)   | 14               | 93                    | 16                | 109                    | 14                                | 93                              | 1.27            | 192           | 701             | 113             |
| 5615        | 2183   | sm(2)    | \-               | \-                    | 16                | 109                    | \-                                | \-                              | 69.73           | 192           | 699             | 113             |
| 5615        | 2183   | inc(3)   | 23               | 161                   | 30                | 215                    | 23                                | 161                             | 5.68            | 192           | 1049            | 145             |
| 5615        | 2183   | sm(3)    | \-               | \-                    | 29                | 209                    | \-                                | \-                              | 103.39          | 192           | 1043            | 145             |
| 5615        | 2183   | inc(4)   | 41               | 316                   | 55                | 436                    | 37                                | 276                             | 16.83           | 192           | 1585            | 178             |
| 5615        | 2183   | sm(4)    | \-               | \-                    | 54                | 430                    | \-                                | \-                              | 135.63          | 192           | 1583            | 179             |
| 5914        | 1.01   | inc(2)   | 14               | 93                    | 15                | 98                     | 14                                | 93                              | 1.01            | 191           | 688             | 115             |
| 5914        | 1432   | sm(2)    | \-               | \-                    | 14                | 93                     | \-                                | \-                              | 79.29           | 191           | 662             | 109             |
| 5914        | 1432   | inc(3)   | 27               | 193                   | 31                | 217                    | 27                                | 193                             | 2.69            | 191           | 1101            | 155             |
| 5914        | 1432   | sm(3)    | \-               | \-                    | 31                | 217                    | \-                                | \-                              | 95.59           | 191           | 1100            | 155             |
| 5914        | 1432   | inc(4)   | 53               | 420                   | 57                | 444                    | 45                                | 336                             | 4.79            | 191           | 1532            | 173             |
| 5914        | 1432   | sm(4)    | \-               | \-                    | 56                | 438                    | \-                                | \-                              | 144.66          | 191           | 1502            | 173             |
| 6050        | 0.73   | inc(2)   | 13               | 92                    | 14                | 98                     | 13                                | 92                              | 0.73            | 190           | 688             | 106             |
| 6050        | 1451   | sm(2)    | \-               | \-                    | 14                | 98                     | \-                                | \-                              | 67.68           | 190           | 678             | 105             |
| 6050        | 1451   | inc(3)   | 28               | 205                   | 29                | 211                    | 28                                | 205                             | 2.40            | 190           | 1130            | 150             |
| 6050        | 1451   | sm(3)    | \-               | \-                    | 29                | 211                    | \-                                | \-                              | 109.75          | 190           | 1132            | 150             |
| 6050        | 1451   | inc(4)   | 54               | 432                   | 55                | 438                    | 47                                | 355                             | 2.61            | 190           | 1600            | 175             |
| 6050        | 1451   | sm(4)    | \-               | \-                    | 54                | 432                    | \-                                | \-                              | 199.07          | 190           | 1589            | 175             |
| 6051        | 1.01   | inc(2)   | 13               | 92                    | 15                | 108                    | 13                                | 92                              | 1.01            | 237           | 827             | 133             |
| 6051        | 2307   | sm(2)    | \-               | \-                    | 15                | 108                    | \-                                | \-                              | 68.33           | 237           | 838             | 135             |
| 6051        | 2307   | inc(3)   | 28               | 205                   | 35                | 259                    | 28                                | 205                             | 5.51            | 237           | 1350            | 181             |
| 6051        | 2307   | sm(3)    | \-               | \-                    | 34                | 253                    | \-                                | \-                              | 123.08          | 237           | 1340            | 181             |
| 6051        | 2307   | inc(4)   | 54               | 432                   | 68                | 552                    | 52                                | 412                             | 20.99           | 237           | 1918            | 214             |
| 6051        | 2307   | sm(4)    | \-               | \-                    | 67                | 546                    | \-                                | \-                              | 161.47          | 237           | 1940            | 214             |
| 6361        | 1.33   | inc(2)   | 14               | 89                    | 16                | 105                    | 14                                | 89                              | 1.33            | 187           | 682             | 110             |
| 6361        | 1562   | sm(2)    | \-               | \-                    | 16                | 105                    | \-                                | \-                              | 77.66           | 187           | 680             | 110             |
| 6361        | 1562   | inc(3)   | 23               | 157                   | 29                | 205                    | 23                                | 157                             | 5.49            | 187           | 1106            | 155             |
| 6361        | 1562   | sm(3)    | \-               | \-                    | 29                | 205                    | \-                                | \-                              | 103.12          | 187           | 1112            | 155             |
| 6361        | 1562   | inc(4)   | 40               | 306                   | 54                | 426                    | 35                                | 254                             | 12.08           | 187           | 1495            | 174             |
| 6361        | 1562   | sm(4)    | \-               | \-                    | 54                | 426                    | \-                                | \-                              | 169.17          | 187           | 1519            | 174             |
| 7119        | 0.81   | inc(2)   | 16               | 108                   | 17                | 113                    | 16                                | 108                             | 0.81            | 201           | 804             | 124             |
| 7119        | 2211   | sm(2)    | \-               | \-                    | 16                | 108                    | \-                                | \-                              | 67.50           | 201           | 805             | 124             |
| 7119        | 2211   | inc(3)   | 29               | 208                   | 33                | 232                    | 29                                | 208                             | 5.96            | 201           | 1132            | 154             |
| 7119        | 2211   | sm(3)    | \-               | \-                    | 33                | 232                    | \-                                | \-                              | 131.86          | 201           | 1139            | 154             |
| 7119        | 2211   | inc(4)   | 55               | 435                   | 59                | 459                    | 48                                | 364                             | 6.44            | 201           | 1629            | 185             |
| 7119        | 2211   | sm(4)    | \-               | \-                    | 58                | 453                    | \-                                | \-                              | 145.04          | 201           | 1631            | 185             |
| 7349        | 0.88   | inc(2)   | 19               | 128                   | 20                | 133                    | 19                                | 128                             | 0.88            | 251           | 943             | 154             |
| 7349        | 2328   | sm(2)    | \-               | \-                    | 19                | 128                    | \-                                | \-                              | 76.54           | 251           | 920             | 149             |
| 7349        | 2328   | inc(3)   | 36               | 260                   | 40                | 284                    | 36                                | 260                             | 2.73            | 251           | 1450            | 205             |
| 7349        | 2328   | sm(3)    | \-               | \-                    | 40                | 284                    | \-                                | \-                              | 157.66          | 251           | 1449            | 205             |
| 7349        | 2328   | inc(4)   | 70               | 559                   | 74                | 583                    | 60                                | 459                             | 7.91            | 251           | 2040            | 235             |
| 7349        | 2328   | sm(4)    | \-               | \-                    | 73                | 577                    | \-                                | \-                              | 200.08          | 251           | 2022            | 233             |
| 7500        | 0.87   | inc(2)   | 11               | 68                    | 12                | 73                     | 11                                | 68                              | 0.87            | 137           | 465             | 80              |
| 7500        | 1803   | sm(2)    | \-               | \-                    | 12                | 73                     | \-                                | \-                              | 62.37           | 137           | 453             | 77              |
| 7500        | 1803   | inc(3)   | 24               | 160                   | 25                | 165                    | 24                                | 160                             | 2.20            | 137           | 727             | 104             |
| 7500        | 1803   | sm(3)    | \-               | \-                    | 25                | 165                    | \-                                | \-                              | 80.32           | 137           | 727             | 104             |
| 7500        | 1803   | inc(4)   | 41               | 309                   | 42                | 314                    | 33                                | 229                             | 3.05            | 137           | 1082            | 129             |
| 7500        | 1803   | sm(4)    | \-               | \-                    | 42                | 314                    | \-                                | \-                              | 126.76          | 137           | 1097            | 129             |
| 8178        | 1.3    | inc(2)   | 18               | 119                   | 19                | 128                    | 18                                | 119                             | 1.30            | 244           | 865             | 142             |
| 8178        | 2279   | sm(2)    | \-               | \-                    | 19                | 128                    | \-                                | \-                              | 86.92           | 244           | 863             | 142             |
| 8178        | 2279   | inc(3)   | 35               | 251                   | 36                | 260                    | 35                                | 251                             | 5.03            | 244           | 1326            | 186             |
| 8178        | 2279   | sm(3)    | \-               | \-                    | 36                | 260                    | \-                                | \-                              | 109.13          | 244           | 1319            | 186             |
| 8178        | 2279   | inc(4)   | 68               | 544                   | 70                | 559                    | 54                                | 404                             | 9.57            | 244           | 2034            | 230             |
| 8178        | 2279   | sm(4)    | \-               | \-                    | 69                | 553                    | \-                                | \-                              | 161.00          | 244           | 1993            | 228             |
| 8577        | 1.28   | inc(2)   | 12               | 82                    | 14                | 93                     | 12                                | 82                              | 1.28            | 143           | 516             | 86              |
| 8577        | 2079   | sm(2)    | \-               | \-                    | 14                | 93                     | \-                                | \-                              | 72.13           | 143           | 512             | 86              |
| 8577        | 2079   | inc(3)   | 21               | 150                   | 23                | 161                    | 21                                | 150                             | 2.83            | 143           | 786             | 115             |
| 8577        | 2079   | sm(3)    | \-               | \-                    | 23                | 161                    | \-                                | \-                              | 85.96           | 143           | 787             | 115             |
| 8577        | 2079   | inc(4)   | 39               | 305                   | 41                | 316                    | 33                                | 245                             | 3.97            | 143           | 1047            | 126             |
| 8577        | 2079   | sm(4)    | \-               | \-                    | 40                | 310                    | \-                                | \-                              | 115.25          | 143           | 1062            | 127             |
| 9379        | 1.47   | inc(2)   | 19               | 130                   | 21                | 150                    | 19                                | 130                             | 1.47            | 272           | 1008            | 159             |
| 9379        | 2655   | sm(2)    | \-               | \-                    | 19                | 134                    | \-                                | \-                              | 75.58           | 272           | 1025            | 160             |
| 9379        | 2655   | inc(3)   | 40               | 286                   | 44                | 318                    | 40                                | 286                             | 4.23            | 272           | 1606            | 216             |
| 9379        | 2655   | sm(3)    | \-               | \-                    | 40                | 294                    | \-                                | \-                              | 135.58          | 272           | 1615            | 216             |
| 9379        | 2655   | inc(4)   | 74               | 585                   | 88                | 711                    | 63                                | 474                             | 12.53           | 272           | 2376            | 260             |
| 9379        | 2655   | sm(4)    | \-               | \-                    | 77                | 627                    | \-                                | \-                              | 179.84          | 272           | 2316            | 257             |
| 9432        | 1.18   | inc(2)   | 20               | 137                   | 21                | 146                    | 20                                | 137                             | 1.18            | 265           | 908             | 145             |
| 9432        | 2413   | sm(2)    | \-               | \-                    | 19                | 130                    | \-                                | \-                              | 79.03           | 265           | 901             | 142             |
| 9432        | 2413   | inc(3)   | 40               | 286                   | 41                | 295                    | 40                                | 286                             | 4.60            | 265           | 1474            | 198             |
| 9432        | 2413   | sm(3)    | \-               | \-                    | 37                | 271                    | \-                                | \-                              | 144.92          | 265           | 1457            | 197             |
| 9432        | 2413   | inc(4)   | 82               | 673                   | 84                | 680                    | 63                                | 474                             | 9.72            | 265           | 2300            | 246             |
| 9432        | 2413   | sm(4)    | \-               | \-                    | 75                | 610                    | \-                                | \-                              | 183.33          | 265           | 2223            | 242             |
| 9436        | 0.76   | inc(2)   | 18               | 130                   | 19                | 136                    | 18                                | 130                             | 0.76            | 253           | 878             | 135             |
| 9436        | 2390   | sm(2)    | \-               | \-                    | 17                | 120                    | \-                                | \-                              | 77.79           | 253           | 888             | 135             |
| 9436        | 2390   | inc(3)   | 37               | 274                   | 38                | 280                    | 37                                | 274                             | 2.55            | 253           | 1448            | 191             |
| 9436        | 2390   | sm(3)    | \-               | \-                    | 34                | 256                    | \-                                | \-                              | 147.35          | 253           | 1456            | 190             |
| 9436        | 2390   | inc(4)   | 78               | 655                   | 79                | 653                    | 68                                | 548                             | 2.39            | 253           | 2219            | 234             |
| 9436        | 2390   | sm(4)    | \-               | \-                    | 71                | 589                    | \-                                | \-                              | 169.32          | 253           | 2167            | 230             |

[Click for the PDF version of the table](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/Data%20on%20TestGeneration%26Execution.pdf)

## Reuse Rates
The table below shows reuse rates of test sequences and events in the testing scenarios. 

| Scenario ID | PUC ID | Test Set | Test Sequences Reused in Test Set/PUC Number of Sequences | Test Sequences Reused in Test Set/Existing Product Number of Sequences | Events Reused in Test Sequences/PUC Number of Events | Events Reused in Test Sequences/Existing Product Number of Events |
| ----------- | ------ | -------- | --------------------------------------------------------- | ---------------------------------------------------------------------- | ---------------------------------------------------- | ----------------------------------------------------------------- |
| 45          | 123    | inc(2)   | 75                                                        | 100                                                                    | 68.62745098                                          | 100                                                               |
| 45          | 123    | inc(3)   | 60                                                        | 100                                                                    | 52                                                   | 100                                                               |
| 45          | 123    | inc(4)   | 41.66666667                                               | 100                                                                    | 32.20338983                                          | 100                                                               |
| 573         | 1005   | inc(2)   | 83.33333333                                               | 100                                                                    | 78.37837838                                          | 100                                                               |
| 573         | 1005   | inc(3)   | 75                                                        | 100                                                                    | 70                                                   | 100                                                               |
| 573         | 1005   | inc(4)   | 57.14285714                                               | 85.71428571                                                            | 58.41269841                                          | 94.35897436                                                       |
| 962         | 210    | inc(2)   | 92.85714286                                               | 100                                                                    | 94.38202247                                          | 100                                                               |
| 962         | 210    | inc(3)   | 95.65217391                                               | 100                                                                    | 96.81528662                                          | 100                                                               |
| 962         | 210    | inc(4)   | 77.5                                                      | 79.48717949                                                            | 91.17647059                                          | 92.6910299                                                        |
| 1341        | 352    | inc(2)   | 91.66666667                                               | 100                                                                    | 92.75362319                                          | 100                                                               |
| 1341        | 352    | inc(3)   | 75                                                        | 100                                                                    | 73.91304348                                          | 100                                                               |
| 1341        | 352    | inc(4)   | 77.77777778                                               | 100                                                                    | 76.69902913                                          | 100                                                               |
| 1658        | 487    | inc(2)   | 81.81818182                                               | 100                                                                    | 78.94736842                                          | 100                                                               |
| 1658        | 487    | inc(3)   | 66.66666667                                               | 100                                                                    | 64                                                   | 100                                                               |
| 1658        | 487    | inc(4)   | 55.26315789                                               | 87.5                                                                   | 57.52508361                                          | 96.08938547                                                       |
| 1706        | 444    | inc(2)   | 90.90909091                                               | 100                                                                    | 92.42424242                                          | 100                                                               |
| 1706        | 444    | inc(3)   | 78.94736842                                               | 100                                                                    | 80.16528926                                          | 100                                                               |
| 1706        | 444    | inc(4)   | 79.31034483                                               | 92                                                                     | 84.31372549                                          | 95.55555556                                                       |
| 2217        | 1412   | inc(2)   | 88.88888889                                               | 100                                                                    | 86.44067797                                          | 100                                                               |
| 2217        | 1412   | inc(3)   | 78.125                                                    | 100                                                                    | 75.89285714                                          | 100                                                               |
| 2217        | 1412   | inc(4)   | 68.42105263                                               | 90.69767442                                                            | 70.78651685                                          | 96.92307692                                                       |
| 2511        | 1493   | inc(2)   | 86.66666667                                               | 100                                                                    | 82.02247191                                          | 100                                                               |
| 2511        | 1493   | inc(3)   | 76                                                        | 100                                                                    | 70.37037037                                          | 100                                                               |
| 2511        | 1493   | inc(4)   | 58.13953488                                               | 86.20689655                                                            | 58.99053628                                          | 94.92385787                                                       |
| 3225        | 1634   | inc(2)   | 84.61538462                                               | 100                                                                    | 81.6091954                                           | 100                                                               |
| 3225        | 1634   | inc(3)   | 69.56521739                                               | 100                                                                    | 66.45962733                                          | 100                                                               |
| 3225        | 1634   | inc(4)   | 60                                                        | 92.30769231                                                            | 59.67741935                                          | 97.36842105                                                       |
| 3445        | 816    | inc(2)   | 92.85714286                                               | 100                                                                    | 95.6043956                                           | 100                                                               |
| 3445        | 816    | inc(3)   | 95.65217391                                               | 100                                                                    | 97.48427673                                          | 100                                                               |
| 3445        | 816    | inc(4)   | 82.92682927                                               | 85                                                                     | 93.94904459                                          | 95.16129032                                                       |
| 3493        | 813    | inc(2)   | 93.33333333                                               | 100                                                                    | 94.38202247                                          | 100                                                               |
| 3493        | 813    | inc(3)   | 96                                                        | 100                                                                    | 96.91358025                                          | 100                                                               |
| 3493        | 813    | inc(4)   | 84.09090909                                               | 86.04651163                                                            | 92.87925697                                          | 94.33962264                                                       |
| 3942        | 1231   | inc(2)   | 90.90909091                                               | 100                                                                    | 86.36363636                                          | 100                                                               |
| 3942        | 1231   | inc(3)   | 95                                                        | 100                                                                    | 92.85714286                                          | 100                                                               |
| 3942        | 1231   | inc(4)   | 80                                                        | 85.71428571                                                            | 87.55980861                                          | 94.32989691                                                       |
| 4365        | 1107   | inc(2)   | 84.61538462                                               | 100                                                                    | 81.17647059                                          | 100                                                               |
| 4365        | 1107   | inc(3)   | 80                                                        | 100                                                                    | 77.03349282                                          | 100                                                               |
| 4365        | 1107   | inc(4)   | 63.63636364                                               | 85.36585366                                                            | 68.37209302                                          | 94.83870968                                                       |
| 4852        | 1116   | inc(2)   | 93.33333333                                               | 100                                                                    | 94.94949495                                          | 100                                                               |
| 4852        | 1116   | inc(3)   | 96.875                                                    | 100                                                                    | 97.75784753                                          | 100                                                               |
| 4852        | 1116   | inc(4)   | 80.70175439                                               | 82.14285714                                                            | 93.24324324                                          | 94.30523918                                                       |
| 4971        | 2027   | inc(2)   | 88.23529412                                               | 100                                                                    | 86.20689655                                          | 100                                                               |
| 4971        | 2027   | inc(3)   | 84.21052632                                               | 100                                                                    | 82.35294118                                          | 100                                                               |
| 4971        | 2027   | inc(4)   | 70.42253521                                               | 87.71929825                                                            | 74.69026549                                          | 94.83146067                                                       |
| 5188        | 1246   | inc(2)   | 92.30769231                                               | 100                                                                    | 93.90243902                                          | 100                                                               |
| 5188        | 1246   | inc(3)   | 80.95238095                                               | 100                                                                    | 82.48175182                                          | 100                                                               |
| 5188        | 1246   | inc(4)   | 77.41935484                                               | 88.88888889                                                            | 85.45454545                                          | 95.91836735                                                       |
| 5283        | 1234   | inc(2)   | 91.66666667                                               | 100                                                                    | 94.66666667                                          | 100                                                               |
| 5283        | 1234   | inc(3)   | 95.23809524                                               | 100                                                                    | 97.03703704                                          | 100                                                               |
| 5283        | 1234   | inc(4)   | 83.87096774                                               | 86.66666667                                                            | 93.57798165                                          | 95.3271028                                                        |
| 5615        | 2183   | inc(2)   | 87.5                                                      | 100                                                                    | 85.32110092                                          | 100                                                               |
| 5615        | 2183   | inc(3)   | 76.66666667                                               | 100                                                                    | 74.88372093                                          | 100                                                               |
| 5615        | 2183   | inc(4)   | 67.27272727                                               | 90.24390244                                                            | 70.18348624                                          | 96.83544304                                                       |
| 5914        | 1432   | inc(2)   | 93.33333333                                               | 100                                                                    | 94.89795918                                          | 100                                                               |
| 5914        | 1432   | inc(3)   | 87.09677419                                               | 100                                                                    | 88.94009217                                          | 100                                                               |
| 5914        | 1432   | inc(4)   | 78.94736842                                               | 84.90566038                                                            | 88.96396396                                          | 94.04761905                                                       |
| 6050        | 1451   | inc(2)   | 92.85714286                                               | 100                                                                    | 93.87755102                                          | 100                                                               |
| 6050        | 1451   | inc(3)   | 96.55172414                                               | 100                                                                    | 97.1563981                                           | 100                                                               |
| 6050        | 1451   | inc(4)   | 85.45454545                                               | 87.03703704                                                            | 93.37899543                                          | 94.67592593                                                       |
| 6051        | 2307   | inc(2)   | 86.66666667                                               | 100                                                                    | 85.18518519                                          | 100                                                               |
| 6051        | 2307   | inc(3)   | 80                                                        | 100                                                                    | 79.15057915                                          | 100                                                               |
| 6051        | 2307   | inc(4)   | 76.47058824                                               | 96.2962963                                                             | 77.35507246                                          | 98.84259259                                                       |
| 6361        | 1562   | inc(2)   | 87.5                                                      | 100                                                                    | 84.76190476                                          | 100                                                               |
| 6361        | 1562   | inc(3)   | 79.31034483                                               | 100                                                                    | 76.58536585                                          | 100                                                               |
| 6361        | 1562   | inc(4)   | 64.81481481                                               | 87.5                                                                   | 68.30985915                                          | 95.09803922                                                       |
| 7119        | 2211   | inc(2)   | 94.11764706                                               | 100                                                                    | 95.57522124                                          | 100                                                               |
| 7119        | 2211   | inc(3)   | 87.87878788                                               | 100                                                                    | 89.65517241                                          | 100                                                               |
| 7119        | 2211   | inc(4)   | 81.3559322                                                | 87.27272727                                                            | 91.06753813                                          | 96.09195402                                                       |
| 7349        | 2328   | inc(2)   | 95                                                        | 100                                                                    | 96.2406015                                           | 100                                                               |
| 7349        | 2328   | inc(3)   | 90                                                        | 100                                                                    | 91.54929577                                          | 100                                                               |
| 7349        | 2328   | inc(4)   | 81.08108108                                               | 85.71428571                                                            | 91.0806175                                           | 94.99105546                                                       |
| 7500        | 1803   | inc(2)   | 91.66666667                                               | 100                                                                    | 93.15068493                                          | 100                                                               |
| 7500        | 1803   | inc(3)   | 96                                                        | 100                                                                    | 96.96969697                                          | 100                                                               |
| 7500        | 1803   | inc(4)   | 78.57142857                                               | 80.48780488                                                            | 91.08280255                                          | 92.5566343                                                        |
| 8178        | 2279   | inc(2)   | 94.73684211                                               | 100                                                                    | 92.96875                                             | 100                                                               |
| 8178        | 2279   | inc(3)   | 97.22222222                                               | 100                                                                    | 96.53846154                                          | 100                                                               |
| 8178        | 2279   | inc(4)   | 77.14285714                                               | 79.41176471                                                            | 90.8765653                                           | 93.38235294                                                       |
| 8577        | 2079   | inc(2)   | 85.71428571                                               | 100                                                                    | 88.17204301                                          | 100                                                               |
| 8577        | 2079   | inc(3)   | 91.30434783                                               | 100                                                                    | 93.16770186                                          | 100                                                               |
| 8577        | 2079   | inc(4)   | 80.48780488                                               | 84.61538462                                                            | 91.4556962                                           | 94.75409836                                                       |
| 9379        | 2655   | inc(2)   | 90.47619048                                               | 100                                                                    | 86.66666667                                          | 100                                                               |
| 9379        | 2655   | inc(3)   | 90.90909091                                               | 100                                                                    | 89.93710692                                          | 100                                                               |
| 9379        | 2655   | inc(4)   | 71.59090909                                               | 85.13513514                                                            | 78.34036568                                          | 95.21367521                                                       |
| 9432        | 2413   | inc(2)   | 95.23809524                                               | 100                                                                    | 93.83561644                                          | 100                                                               |
| 9432        | 2413   | inc(3)   | 97.56097561                                               | 100                                                                    | 96.94915254                                          | 100                                                               |
| 9432        | 2413   | inc(4)   | 75                                                        | 76.82926829                                                            | 91.76470588                                          | 92.7191679                                                        |
| 9436        | 2390   | inc(2)   | 94.73684211                                               | 100                                                                    | 95.58823529                                          | 100                                                               |
| 9436        | 2390   | inc(3)   | 97.36842105                                               | 100                                                                    | 97.85714286                                          | 100                                                               |
| 9436        | 2390   | inc(4)   | 86.07594937                                               | 87.17948718                                                            | 95.55895865                                          | 95.26717557                                                       |

[Click for the PDF version of the table](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/ReuseRates.pdf)
