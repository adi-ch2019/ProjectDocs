# Valuelabs AvidPay - Client Liason - Knowledge Transition wikis

## Identify Information Technology

[]

### Current State of Existing Tech Environment

* Web UI/services Internal support portals for Customer Care & Payments Teams
  * AvidPay
  * Bank Channel Platform - Nacha 2.0 or Hub AvidPay
  * Common

* Servers - On Premises
  * Microsoft Windows Server 2008 R2
  * Ubuntu 12.04
  * Red Hat Enterprise Linux 7
  * Others like Pheonix
  

#### AvidPay

    * Legacy 
    * AvicPay Current State - System Architecture- need to put link of diagram from DevOps

#### BCP 

      * Built out to be Microservice based
      * BAI2 - American Banking Standard for reconciliation files
         All Comprise One function of AvidPay
         Pull BAI2 file from their system to our database

#### Business Impact

    Something is down it is important to know what priority it should be.
    External portal is down and customers cannot login its like a P1

#### Notes
      DevOps Dashboard - organization tags - filter down to say example Octopus
      RCA - go to LoadBalancer - Steps it took and go into the service
      Legacy code AvidPay mostly exists on WEB07 and WEB08
      Internal & External portals get updated frequently. Rest not so much.
      Wednesday nights and Saturday nights - Deployments. 

      Service now 

#### Troubleshooting

* Service Now
  1. avidxchange.service-now.com/nav_to.do?uri=%2Fhome.do%3F
    1. Change
      1. All
       filter down by "Business Service" -> "AvidPay" 

* Application Errors
  1. Octopus Dashboard 
    1. octopus.avidxchange.com
      1. Check last deployment
        1. Project group - "Pay" 
        1. Check relevant api/webapp
        1. Releases
          1. Each step shows a box to which it got deployed to.

* Netscalar
  1. Tr

* Neuron 
    WSO2 - Linux - PoC needed
* Nacha-jobs
  * Legacy
  * Everything else is BCP
  * "Core-debit file change" issues
  * ssch01 server - Windows client 
    * History - jobs/timeframes
    * Monitor - Actively running jobs
    * Production\AvidPay|MoneyFlow

* Redis - pending - when devs are looking for; not necessarily skillset
  * Command Line Utility

* Dynatrace
  Notification button on top left -> Problems
  PurePaths on servers 
  Custom Multidimentional Analysis


* AppInsights 
 * Legacy insights is for Analsis
 * Graphana link 
 * CDE 

* 



