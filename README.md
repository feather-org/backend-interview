# Feather SDE Backend Interview

## Background

Feather is a modern retirement benefits provider for startups in the US. We have launched our first product that makes it easy and affordable for startups to offer a 401(k) plan without worrying about compliance and payroll 💸

We are a high-growth, venture backed startup. We are fortunate to have great investors like Y Combinator and others.

We are a remote-first team with a focus on delivering high quality work. Our distributed nature enables us to expand our team in several locations, gain access to individuals with specialized skills, and support them for continued success. What this means is:
* 💰 High Compensation: We hire the best and pay them accordingly
* 💸 Retirement Benefits (US employees): We offer 401(k) to help you invest in your future
* 🏖️ Location Flexibility: As long as you can work asynchronously with rest of the team
* 🏖️ Unlimited, Untracked PTO: We care about your work, not hours
* 💻 Work Station: We are ready to provide you the tools that help you deliver
* 🍹 Quarterly Retreats: And if you can’t make it, we will still spend on you to have a relaxing time at home

## Interview

### Requirements

This is a take home project for the role of a backend engineer at Feather. This should not take more than 2 hours.

* Set up a new service in any language (preferably Java, Kotlin or Python)
* Set up logging
* Set up the following API endpoints against a database (preferably Dynamo). Note, you can run a local dynamo instance

| Type                      |  Endpoint   | Notes                                          |
|:--------------------------|:-----------:|:-----------------------------------------------|
| GET                       | `/company`  | Return Company                                 |
| POST                      | `/company`  | Returns the unique company id                  |
| POST                      | `/employee` | Returns the unique employee id                 |
| GET all employees         | `/employee` | Returns the paginated Employees (10 at a time) |

* A README file describing how to start / stop the server
* The JSON test cases that were used against the server

### Data Model

Company
* Legal Name
* Incorporation Date
* Display Name
* US State of Incorporation (For example: California)

Employee
* First Name
* Last Name
* Company ID
* Work Email
* Manager ID
* Date of Birth
* Employee Number
* Tax ID Number
* Employment Status: One of ACTIVE and INACTIVE
* Marital Status: One of SINGLE, MARRIED, COMMON LAW, DIVORCED and WIDOWED
