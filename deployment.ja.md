# Deployment check

> **Part of the Multi-team Software Delivery Assessment** ([README](README.md))
> 
> Copyright © 2018-2019 [Conflux Digital Ltd](https://confluxdigital.net/)
> 
> Licenced under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) ![CC BY-SA 4.0](https://licensebuttons.net/l/by-sa/3.0/88x31.png)
>
> _Permalink: [SoftwareDeliveryAssessment.com](http://SoftwareDeliveryAssessment.com/)_ 

Based on the maturity questions from Mirco Hering, author of [*DevOps for the Modern Enterprise*](https://notafactoryanymore.com/2018/03/01/mircos-self-assessment-questions-of-devops-maturity/)

Purpose:  *Assess the confidence of the team in the deployment practices for its software*

Method: Use the [*Spotify Squad Health Check*](https://labs.spotify.com/2014/09/16/squad-health-check-model/) approach to assess the team's answers to the following questions:

| **Question**                                                                                                                                 | **Tired (1)**                                                        | **Inspired (5)**                                             |
| -------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------- | ------------------------------------------------------------ |
| 1\. **Environment Rebuild** - What would happen if we decided to: **blow away the environment and rebuild it from our stored configuration** | We don't know what would happen - the environments are flaky         | No problem - we test this in the deployment pipeline already |
| 2\. **Fresh Config** - What would happen if we decided to: **delete the application config and redeploy it**                                 | We don't know what would happen - the configuration process is flaky | No problem - we test this in the deployment pipeline already |
| 3\. **Redeploy App** - What would happen if we decided to: **redeploy the application even though nothing has changed**                      | We don't know what would happen - the deployments are flaky          | No problem - we test this in the deployment pipeline already |
| 4\. **Rerun Tests** - What would happen if we decided to: **rerun the test suite and then again**                                            | We don't know what would happen - the test suite is really flaky     | No problem - we test this in the deployment pipeline already |

