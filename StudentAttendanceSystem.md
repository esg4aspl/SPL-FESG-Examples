# Student Attendance System

Student Attendance System product line has 20 features and a core feature. The core of the product line represents the common behavior which exists in all products that belong to Student Attendance System product line. The core behavior is modelled using core ESG (c-ESG). An optional behavior is modelled using a feature ESG (f-ESG). A featured ESG (FESG) is an extended ESG that is composed of a core ESG (c-ESG) and a set of feature ESGs (f-ESGs). A featured ESG is used in test sequence composition approach which composes the sequences of core and feature ESGs and generates a product's test sequences. The models of Student Attendance System product line are built from the users' perspective. The Event Sequence graphs' events are selected from user events.

## Feature Model

![Feature Model](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_ModelImages/StudentAttendanceSystemPL_featureModel.png)\
This feature model has 6 mandatory abstract features which means that at least or exactly one of their subfeatures has to be included in each product configuration. In this feature model various constraints are included such as the feature _edit schedule_ implies the feature _add new schedule_. 2664 different product configurations could be obtained by combining these features and applying the constraints of the feature model.

## Student Attendance System Products
There are 2664 product configurations in Student Attendance System Product Line. Due to the space concerns, we don't put all of the product information here. In the table below, the product id and the belonging features are given. Since, each possible product does not have a unique official name, we assign IDs to products to name them uniquely.

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

# Student Attendance System Product Line Features
## Core ESG (c-ESG)
 ![core](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystem/StudentAttendanceSystemPL_ModelImages/core.PNG)\
 The core ESG of the elevator product line represents core features, which exist in all product configurations. For this product line the core feature is composing a new email, sending an email and receiving an email. Note that, the product that has the ID 0, has only core feature since the core feature itself, is capable of generating test sequences.\
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
