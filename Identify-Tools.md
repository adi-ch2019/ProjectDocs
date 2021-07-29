
Identify Tools

Site server tools can be utilised to build, host, track and monitor transactions on a business site. There are a wide range of possibilities. The categories considered in this resource are:

    Statistical analysis tools to analyse website usage
    Payment processing tools
    File synchronisation tools

Statistical Analysis

The analysis of web server logs will add great value to the business and its management behind any site. These logs (which have to be switched on to be used) offer a variety of useful information such as:

    How many visitors?
    How many unique visitors?
    Where (which country) did they come from?
    What are their screen resolutions?
    What browser do they favour?
    What pages were visited and for how long?
    Did any robots / spiders visit the site?
    What is the peak traffic period and how much bandwidth does it consume?

Built in web server logging tools

Web servers such as Apache and MS IIS provide built-in site activity logging functionality to provide information such as:

    Who has accessed the website?
    When was it accessed?
    What was accessed?

This information can make it possible to identify bottlenecks, security breaches, content popularity and facilitate troubleshooting.

The W3C specification for extended log file format, describes a number of log fields that can be used for web server activity logging. The specification calls for an ASCII file format and time is logged as UTC (Greenwich Mean Time).

A selection of the properties that can be logged are described in the table below:
Field 	Description
Date 	Date activity occurred
Time 	Time activity occurred
Client IP address 	The IP address of the client computer
Username 	The username of the person who accessed the server
Service 	The Internet service that was accessed
Port 	The port number the client connected to
Method 	The action (such as HTTP GET) that the user was performing
URI stem 	The resource (eg webpage.htm) accessed
Time taken 	The length of time the action took
User agent 	The client browser used
Cookie 	The content of any cookies sent or received
Referrer 	Previous site visited by user

Further details can be found at http://www.w3c.com

Complete Activity 2: Server tools

Activity icon
Activity 2

Complete Activity 3: Server log statistics

Activity icon
Activity 3

Complete Activity 4: Setting up server logs

Activity icon
Activity 4

Processing payments online (E-commerce).

Online credit card payment processing, (currently the most popular system on the internet), offers a range of alternatives that may be influenced by the volume and / or budget of the sales in question.

    Low volume and / or low budget sales
    PayPal, Pay Mate, Worldpay, iKobo, iBill or similar system or manual credit card processing
    High volume and / or high budget sales
    Real time credit card payments or manual credit card processing

A PayPal account (or equivalent) is by far the easiest system to implement. The system involves setting up an account and posting information to its payment gateway via an online form.

Manual credit card processing involves a customer providing you with their credit card details on their order, the site may choose to store these details in a secure location for later purchase processing, (the sites privacy policy should be consulted in this instance, so as not to alienate the customer by using these stored details inappropriately). These payments will then be manually processed offline with the company bank.

Real time processing of credit card information will require a Merchant Bank Account. Most Bricks and Mortar companies will have an existing bank infrastructure in place. This facility may be expanded to cater for online processing. The merchant account will also require the completion of a Merchant Agreement, which facilitates the processing of credit card transactions over the internet or over the phone, also known as MOTO (Mail Order Telephone Order). The difference between a MOTO agreement and a normal over the counter agreement is who accepts liability. The MOTO agreement attaches the liability of fraudulent transaction to the merchant not the bank. In order to cover this potential fraud, a merchant fee with a value of 2 - 4% (in Australia) is assigned to each credit card transaction by the card issuer.

As an alternative to the company's existing bank, other external providers may offer more attractive packages, (eg. lower transaction fees, more features), therefore, shopping around via an internet search should be considered to present an informed source of management data in relation to real time credit card processing.

When credit card information is collected online, it should be done over a secured line. This is equally true of processing C2C (Consumer to Consumer) or EDI (Electronic Data Interchange) information via an extranet.

Currently the most common approach is SSL or the Secured Sockets Layer, characterised by the https:// protocol. As a prerequisite, this SSL facility requires the purchase of a Digital Certificate from a provider such as Verisign, Thawte, GeoTrust or equivalent. (These organisations provide a facility that vouches for the owner of the certificate, in effect, saying they are who they say they are.)

This certificate is then installed on a server and used to encrypt / decrypt data over the https:// connection using public and private key encryption techniques. Included in the purchase of the certificate is the number of bits used in the encryption method, (the most common being 40 and 128 bits).

The more bits used, the more secure the encryption method, the more the certificate will cost and the more real time processing power needed to encrypt the data on the page. Note: Some financial organisations require 128 bit encryption.

Complete Activity 5: Digital certificates

Activity icon
Activity 5

Using a payment gateway provider

Using a payment gateway provider may prove to be a more realistic approach to processing real time credit card information, as they offer a range of connection alternatives. In simple terms, they allow the site to scale as it grows:

    By providing a shared SSL connection (no owner digital certificate required)
    Alternately they allow the use of the users own digital certificate on their server
    They may also provide other information not provided by the banking institution
    By providing a range of shopping cart implementations to use within the website itself

Complete Activity 6: Payment gateways

Activity icon
Activity 6

Start simple?

A modest starting point using a simple PayPal account (or equivalent) may well prove to be a worthwhile venture, particularly if sales volumes are unknown. The website design may be scaled up over time, in response to the statistical analysis of monitored data. Remember, the more a site caters and changes to meet its demands, generally the more successful the site.

Implementation budget and time constraints will also impact on tool selection.

Currently one very hot discussion topic is open source software, as it is generally freeware or has a minimal associated charge. Open source tools will greatly favour a tight budget, at least on the surface, however, extra time should be factored into the implementation to cover undocumented features that may be exposed in their use within the specified environment or alternatively the degree of difficulty with the setup process itself.

The other major open source benefit is that the source code is available for customisation or contribution by the user. This may not be a trivial matter and so programming language choice should be factored into the selection criteria if this is deemed an important issue.

It should also be noted that to customise an existing product, total familiarisation with that product should be achieved first, as the feature you may want to implement may already be part of the product and require only runtime switch changes for activation.

An excellent or rather the definitive source of Open Source software is Source Forge http://www.sourceforge.net, although it can be an overwhelming experience navigating through the amassed content. As a suggestion use the software map (tab) page to perform your searches within the site.

Sourceforge Page

[click on image for a larger view]

This powerful search facility is a must for the site's navigation. Try filtering by Operating System or language and then by topic to provide a more contextual reference point.

However, to use the advanced searching facilities and therefore getting the most out of this resource, Source Forge requires a subscription fee of $39 US per annum. If you intend to use this site as your main resource, this small sum may be money well spent.

Data file synchronisation

The ability to manage file systems graphically is a proven productivity boost to anyone that has tried to manually synchronise remote machines via command line programs / shells such as telnet. Most website integrated development environments will feature some basic FTP functionality. Some operating systems provide these features for free but other tools may have to be sought to do more specific tasks such as the synchronisation of a mySQL database between a development machine and a production server.

One such tool is SQLYog http://www.webyog.com. The interface is shown in the graphic below:

 

SQL Yog

Other synchronisation tools offer file size and timestamp comparison; some even go as far as byte by byte comparison.

Complete Activity 7: Graphical file systems

Activity icon
Activity 7

^ top
