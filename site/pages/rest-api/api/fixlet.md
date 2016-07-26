---
title: RESTAPI Fixlet
---

{% restapi "fixlets/{site type}/{site name}", "GET", "Fetches a list of Fixlets of a particular site." %}
 - /api/fixlets/master --> returns fixlets from the master action site
 - /api/fixlets/custom/MyCustomSite --> returns fixlets from your MyCustomSite custom site.
 - /api/fixlets/external/BES Support --> returns fixlets from the external site "BES Support"
 - /api/fixlets/operator/Daniel --> returns fixlets from Daniel's operator site
 
**Request:** URL is all that is required

**Response:** BESAPI description of contained Fixlet resources.

**Response Schema:** BESAPI.xsd
{% endrestapi %}

{% restapi "fixlets/{site type}/{site name}", "PUT", "Not Supported" %}
{% endrestapi %}

{% restapi "fixlets/{site type}/{site name}", "POST", "Creates a fixlet in the specified site." %}
**Request:** Complete XML for the object in the body of the request

**Request Schema:** BES.xsd

**Response Schema:** BESAPI.xsd
{% endrestapi %}

{% restapi "fixlets/{site type}/{site name}", "DELETE", "Not Supported" %}
{% endrestapi %}

{% restapi "fixlet/{site type}/{site name}/{fixlet id}", "GET", "Returns the details of the specified Fixlet." %}
**Request:** URL is all that is required 

**Response:** XML of Fixlet

**Response Schema:** BES.xsd
{% endrestapi %}

{% restapi "fixlet/{site type}/{site name}/{fixlet id}", "PUT", "Updates a Fixlet." %}

**Request:** Complete XML for the object in the body of the request

**Request Schema:** BES.xsd

**Response:** Fixlet ID.

**Response Schema:** Plain text.
{% endrestapi %}

{% restapi "fixlet/{site type}/{site name}/{fixlet id}", "POST", "Creates a Fixlet in the specified site." %}
**Request:** Complete XML for the object in the body of the request

**Request Schema:** BES.xsd

**Response Schema:** BESAPI.xsd
{% endrestapi %}

{% restapi "fixlet/{site type}/{site name}/{fixlet id}", "DELETE", "Deletes a Fixlet." %}
The same command applies to a task if you specify the task ID in place of the Fixlet ID.

**Request:** URL is all that is required
{% endrestapi %}

{% restapi "fixlet/{site type}/{site name}/{fixlet id}/computers", "GET", "Lists the computers that are relevant for this Fixlet." %}
**Request:** URL is all that is required

**Response:** XML  list of computers.
	
**Response Schema:** BESAPI.xsd
{% endrestapi %}

{% restapi "fixlet/{site type}/{site name}/{fixlet id}/computers", "PUT", "Not Supported" %}
{% endrestapi %}

{% restapi "fixlet/{site type}/{site name}/{fixlet id}/computers", "POST", "Not Supported" %}
{% endrestapi %}

{% restapi "fixlet/{site type}/{site name}/{fixlet id}/computers", "DELETE", "Not Supported" %}
{% endrestapi %}