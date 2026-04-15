# Data Egress

This document is focused on data egress methods supported by the DSH platform.

## Introduction
Data Egress is the process of moving data out of a system. For the DSH, egress means the controlled one-way exit used to extract datasets, code, or files from the DSH. Because the environment is isolated, protected and regulated, users cannot extract or copy information out of it without permission. A formal egress mechanism and procedure is used.

The aim of a secure egress process is to ensure that no data passes through the airlock into a public workstation without full statistical disclosure checking and approval.

!!! info

    Disclosure Control is used to protect confidentiality in released data. 
    It ensures that individuals, households, or organizations cannot be identified from results, 
    such as tables or graphs, while maintaining the accuracy and utility of the data.

## Disclosure Checks
Disclosure checking is carried out by [Data Connect](https://sheffield.ac.uk/data-connect) at the University of Sheffield to ensure no sensitive information is removed from the DSH.

## Output checking process

The output checking procedure for University of Sheffield users of the DSH is as follows:

1. A DSH user identifies the specific files needed to be egressed and moved them to a dedicated S3 storage bucket.
2. Whether the information is safe to be moved out of the environment is discussed with the PI or the IAO.
3. Once the PI / IAO has agreed on the egress request, a formal request is submitted to Data Connect to begin the statistical disclosure checking of the proposed outputs.
4. Data Connect will carry out full disclosure checks on the proposed data to be egressed.
5. Once approved Data Connect will make a formal request for egress to the SDS by raising a topdesk ticket.
6. Data Connect moves the files into a dedicated bucket created by the SDS and confirms transfer. SDS will then disable the bucket to prevent the user from uploading extra files.
7. The files will undergo manual checks that ensure everything is fully aligned with what’s been agreed. If during the checks SDS identifies potential risks or information that has not been approved to be moved out of DSH, the request will be denied and the process will have to be repeated from the start.
8. Once the checks are completed and there are no issues with the information, the requester (PI / AIO) will receive an email with an encrypted .zip file containing the files.
9. After the requester has informed SDS that the .zip file has been received, a second email containing the password of the .zip file will be sent. That ensures that an unauthorised user will not, by accident, receive both the .zip and the password to unlock it. The requester should inform SDS as soon as possible if the file or the password has not been received. 




