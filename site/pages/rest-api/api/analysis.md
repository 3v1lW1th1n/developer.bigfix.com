---
title: Analysis
---

{% restapi "analyses/{site type}/{site name}", "GET", "Fetches a list of analyses in the specified site." %}
**Request:** URL is all that is required.

**Response:** XML list of Analysis.

**Response Schema:** BESAPI.xsd
{% endrestapi %}

{% restapi "analyses/{site type}/{site name}", "PUT", "Not Supported" %}
{% endrestapi %}

{% restapi "analyses/{site type}/{site name}", "POST", "Create an analysis in the specified site." %}
**Request:** Complete XML for the objects in the body of the request.

**Request Schema:** BES.xsd

**Response Schema:** BESAPI.xsd
{% endrestapi %}

{% restapi "analyses/{site type}/{site name}", "DELETE", "Not Supported" %}
{% endrestapi %}


{% restapi "analysis/{site type}/{site name}/{analysis id}", "GET", "Get the XML for a specific analysis." %}
**Request:** URL is all that is required.

**Response:** BES XML of Object

**Response Schema:** BES.xsd
{% endrestapi %}

{% restapi "analysis/{site type}/{site name}/{analysis id}", "PUT", "Update an analysis." %}
**Request:** Complete XML for the object in the body of the request.

**Request Schema:** BES.xsd

**Response:** Analysis ID number.
{% endrestapi %}

{% restapi "analysis/{site type}/{site name}/{analysis id}", "POST", "Create an analysis with the supplied XML in the specified site." %}
**Request:** Complete XML for the object in the body of the request.

**Request Schema:** BES.xsd

**Response Schema:** BES.xsd
{% endrestapi %}

{% restapi "analysis/{site type}/{site name}/{analysis id}", "DELETE", "Delete and deactivate an analysis." %}
**Request:** URL is all that is required.
{% endrestapi %}

{% restapi "analysis/{site type}/{site name}/{analysis id}/activations", "GET", "List of analysis activations." %}
**Request:** URL is all that is required.

**Response:**  XML for list of activations. 

**Response Schema:** BESAPI.xsd
{% endrestapi %}

{% restapi "analysis/{site type}/{site name}/{analysis id}/activations", "PUT", "Not supported" %}
{% endrestapi %}

{% restapi "analysis/{site type}/{site name}/{analysis id}/activations", "POST", "Create a new activation for the current operator." %}
**Request:** No body is required, the activation will be created as the operator making the request.

**Response:** XML for the activation. This is relevant to IBM BigFix V9.2 and later.

**Response Schema:** BESAPI.xsd
{% endrestapi %}

{% restapi "analysis/{site type}/{site name}/{analysis id}/activations", "DELETE", "Deletes all activations for the specified analysis." %}
**Request:** URL is all that is required.
{% endrestapi %}

{% restapi "analysis/{site type}/{site name}/{analysis id}/activation/{activation id}", "GET", "Gets analysis activation details." %}
**Request:** URL is all that is required.

**Response:**  Activation details.

**Response schema:** BESAPI.xsd.
{% endrestapi %}

{% restapi "analysis/{site type}/{site name}/{analysis id}/activation/{activation id}", "PUT", "Not supported" %}
{% endrestapi %}

{% restapi "analysis/{site type}/{site name}/{analysis id}/activation/{activation id}", "POST", "Not supported" %}
{% endrestapi %}

{% restapi "analysis/{site type}/{site name}/{analysis id}/activation/{activation id}", "DELETE", "Deactivates a specific analysis activation." %}
**Request:** URL is all that is required.
{% endrestapi %}
