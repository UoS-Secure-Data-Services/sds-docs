# Data Egress

This document is focused on data egress methods supported by the DSH platform.

## Introduction
Data Egress is the process of moving data out of a system. For the DSH, egress means the controlled  exit used to extract datasets, code, or files from the DSH. Because the environment is isolated and secure users cannot extract or copy information out of it without permission, a formal egress mechanism and procedure is used.

The aim of a secure egress process is to ensure that no data passes through the airlock into a public workstation without full statistical disclosure checking and approval.

!!! info

    Disclosure Control is used to protect confidentiality in released data. 
    It ensures that individuals, households, or organizations cannot be identified from results, 
    such as tables or graphs, while maintaining the accuracy and utility of the data.

## Disclosure Checks
Disclosure checking is carried out by [Data Connect](https://sheffield.ac.uk/data-connect) at the University of Sheffield to ensure no sensitive information is removed from the DSH.

For examples of disclosure rules using patient data see [NHS methodology](https://digital.nhs.uk/data-and-information/data-tools-and-services/data-services/hospital-episode-statistics/disclosure-control-methodology-for-hospital-episode-statistics-and-emergency-care-data-set) for egressing results based on Hospital Episode Statistiscs from a secure data environment.

## Output checking process

The output checking procedure for University of Sheffield users of the DSH is as follows:

1. A DSH user identifies the specific files needed to be egressed. The files should be agreed with the principal investigator (PI) or the information asset owner (IAO). 
2. A formal request is submitted via email to Data Connect to begin the statistical disclosure checking of the proposed outputs.
3. The researchers should create a dedicated S3 storage bucket within their project environment named '[ProjectID]-Output-Checking', with a clearly named folder ([submission-number]-[version-number]) as agreed with Data Connect. Requested outputs should be moved here.
4. Data Connect will carry out full disclosure checks on the proposed data to be egressed.
5. Once approved, Data Connect will make a formal request for egress to the Secure Data Service (SDS) by raising a topdesk ticket.
6. Data Connect moves the files into an additional dedicated S3 bucket created by the SDS and confirms transfer.
7. SDS will disable the bucket to prevent the DSH user from uploading additional files.
8. The files will undergo manual checks that ensure the correct files are present. If during the checks SDS identifies potential risks or information that has not been approved to be moved out of DSH, the request will be denied and the process will have to be repeated from the start.
9. Once the checks are completed and approved, the requester (PI / AIO) will receive an email with an encrypted .zip file containing the files.
10. After the requester has informed SDS that the .zip file has been received, a second email containing the password of the .zip file will be sent. That ensures that an unauthorised user will not, by accident, receive both the .zip and the password to unlock it. The requester should inform SDS as soon as possible if the file or the password has not been received. 
