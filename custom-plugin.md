---
layout: post
category : Custom MOTECH module
tags : [module, motech, motechsuite, tutorial]
---
{% include JB/setup %}

## Overview 

### MOTECH module?


### Examples





MOTECH expects:

    .
	|-- pom.xml
    |-- src
        |-- main
            |-- java
			|-- resources
				|-- META-INF
				|   |--osgi 
				|   |  |-- applicationContext.xml
				|   |--spring 
				|      |-- applicationBundleContext.xml
				|-- webapp
					|-- index.html
					|-- messages
					|-- css
					|-- js
					|	|-- app.js
					|	|-- controllers.js
					|	|-- services.js
					|-- partials
						|-- frame.html


- **osgi\applicationContext.yml**  
	Spring application context for non osgi beans.

- **\applicationBundleContext.xml**  
	Spring application context for spring bundles.

- **\webapp**   
	Resource folder for static web resources like html css js etc

- **\webapp\partials**  
	Partial angular html fragments


### POM Configuration


#### Context-Path
Directive for module context path in url, 
ex: callFlow will map url to `http://host:port/motech-platform-server/module/callFlow`





Please take a look at [{{ site.categories.api.first.title }}]({{ BASE_PATH }}{{ site.categories.api.first.url }}) 
or jump right into [Usage]({{ BASE_PATH }}{{ site.categories.usage.first.url }}) if you'd like.