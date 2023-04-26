# 101 Ways Bounded Context Canvas Template

Created: Grant Smith

Created at: February 4, 2022

# <Name> bounded context canvas

# Description

>What benefits does this context provide and how does it provide them

# Ubiquitous language

>Context specific domain terminology

- *Domain term: Definition*
- *Domain term: Definition*
- *Domain term: Definition*

# Inbound data
### Data provided by another context
```yaml
# employee data
   employee_id: 1234
    name: John Smith
     contact: 
       home: 02012345678
       office: 02087654321
     role: Software Engineer
     office_address: 
       street: "145 City Rd"
       town: London
       post_code: EC1V 1AZ
     employed: True
```
### Data provided by another context

```yaml
# skills data
   employee_id: 1234
   skills:
     - Javascript
     - Azure
     - Github Actions
```
## Events consumed
- EmploymentStatusUpdated
- EmployeeSkillsUpdated

# Business rules

1. If skills include 'Azure' raise event AzureDevOps
2. ...

# Outbound Data
```yaml
# Talent Availability Object
employee_id: 1234
   skills:
     - Javascript
     - Azure
     - Github Actions
   Region: SE
   available_for_work: True
   work_type: [ "Front-end Engineering", "DevOps" ]
```
## Events published
- FrontendEngineerAvailable
- DevOpsEngineerAvailable 

# Assumptions

Talent team are specifically interested in Azure DevOps capability