# Flow check

> **Part of the Multi-team Software Delivery Assessment** ([README](README.md))
> 
> Copyright © 2018-2019 [Conflux Digital Ltd](https://confluxdigital.net/)
> 
> Licenced under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) ![CC BY-SA 4.0](https://licensebuttons.net/l/by-sa/3.0/88x31.png)
>
> _Permalink: [SoftwareDeliveryAssessment.com](http://SoftwareDeliveryAssessment.com/)_ 

Based on the key assessment criteria from [*Accelerate*](https://wordery.com/accelerate-nicole-forsgren-phd-9781942788331) by Nicole Forsgren, Jez Humble, and Gene Kim plus detail from [*Principles of Product Development Flow*](https://wordery.com/the-principles-of-product-development-flow-donald-g-reinertsen-9781935401001) by Don Reinertsen

Purpose: *Assess the awareness and performance of the team regarding end-to-end delivery metrics*

Method: Use the [*Spotify Squad Health Check*](https://labs.spotify.com/2014/09/16/squad-health-check-model/) approach to assess the team's answers to the following questions, and also
capture the answers:

| **Question**                                                                                                                                                                    | **Tired (1)**                                                              | **Inspired (5)**                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1\. **Cycle Time** - How long does it take for a code change to go from version control to running in Production? (Minimum, Typical)                                            | 2 weeks or more                                                            | 1 hour or less                                                                                                                                      |
| 2\. **Deployment Frequency** - How often does your team deploy to Production?                                                                                                   | Every 2 weeks or longer in practice                                        | Every 2 days or less                                                                                                                                |
| 3\. **MTTR** - How long does it take to restore your application or service after an incident?                                                                                  | We have no idea - we do not track this                                     | We track MTTR and we restore service in 10 mins automatically and test this in the deployment pipeline                                              |
| 4\. **Failed Changes** - What proportion of changes to your application or service in Production fail or need remediation? (This is typically the number of failed deployments) | More than 20% of our changes/deployments fail in Production                | Less than 5% of our changes/deployments fail in Production                                                                                          |
| 5\. **Work in Progress** - How many things does your team work on at the same time? (Minimum, Typical)                                                                              | We have significantly more Work In Progress (WIP) items than team members  | We have explicitly limited our WIP based on queuing theory (or Cost of Delay) and the WIP is equal to or less than the number of people in our team |
| 6\. **Innovation** - How well are you able to innovate around delivery approaches?                                                                                              | We do not have time to innovate                                            | We make or reserve time for delivery innovation every week and track progress as part of our team metrics                                           |
| 7\. **Onboarding** - How effective is the onboarding process for new teams and new staff?                                                                                       | The onboarding process is incredibly difficult and really hampers progress | The onboarding process is very simple, straightforward, and clear.                                                                                  |
| 8\. **Branch Age** - How long do your branches live? (other than *master*)                                                                                                      | Our feature branches last for many sprints                                 | We develop directly on master/trunk and any feature branches last no more then 2 days                                                               |
| 9\. **Retrospectives** - How effective are your team retrospectives?                                                                                                            | We do not have regular retrospectives                                      | Our retrospectives are really energising/valuable/effective for the team and we look forward to them                                                |

