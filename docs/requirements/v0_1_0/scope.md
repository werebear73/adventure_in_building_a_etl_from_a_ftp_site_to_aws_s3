# Scope

## Project Statement of Purpose
This project is to move the daily file from a FTP site to a AWS S3 bucket for further processing which is not in the scope of the project.

## Objective
| ID | Objective |
|:---:|:---|
|OBJ01|Move the daily file from the FTP site to the S3 Bucket|

## Project Assumptions
| ID | Assumptions |
|:---:|:---|
|AS01|The daily file will always be there at the prescribed time.|
|AS02|The FTP site will always be available at the prescribed time.|
|AS03|The AWS S3 will always be available at the prescribed time.|

## Project Constraints
| ID | Constraints|
|:---:|:---|
|CO01|Make the process as cheap as possible.|

## External Interactions
### Context Level Dataflow Diagram
![Context Level Dataflow Diagram](context_level_dataflow_diagram.svg)

### Textual Context Level Dataflow
| ID  | External Agent | Data Coming From EA |  Data Going To EA  |
| --- | -------------- | ------------------- | ------------------ |
| DF1 | FTP Site       | Data File (Zipped)  |                    |
| DF2 | AWS S3         |                     | Data File (Zipped) |

## Items Out of Scope
| ID | Items Out of Scope |
|:---:|:---|
|OOS01| Processing of the file after it is in the AWS S3 |
|OOS02| Trying to transfer files that may not been missed |
|OOS03| Trying to transfer files that on the FTP prior to the application development |

## Project Stackholders
| Name | Title | Role |
|:---:|:---:|:---:|
| Sam Ware | Owner of Waretech Services | Business Analyst and Developer |
| Undisclosed Individual | Project Lead | Project Owner |

## Glossary
| ID | Term | Definition |
|:---:|:---:|:---:|
|GL01|||