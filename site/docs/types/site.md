# type: site

A &lt;site&gt; object is provided to access properties of Fixlet sites.

# client folder of &lt;site&gt;

The folder containing the site content on the client machine. Site content is gathered into this location.

# evaluated of &lt;site&gt;

No documentation exists.

# fixlet of &lt;site&gt;

Iterates through the Fixlet messages of the specified site.

# folder of &lt;site&gt;

No documentation exists.

# gather schedule authority of &lt;site&gt;

Returns a string corresponding to the authority of the site schedule, for example: Publisher, Custom, Manual or Disabled.

# gather schedule time interval of &lt;site&gt;

Returns the time interval between automatic gathering of site content.

# group &lt;integer&gt; of &lt;site&gt;

Returns an object corresponding to the numbered group of the specified site.

# last gather time of &lt;site&gt;

Returns the time of last successful gathering from the site.

# masthead of &lt;site&gt;

Each site has a masthead, and the masthead is saved into the site data folder upon successful creation. This property returns a file object that corresponds to the copy in the site data folder.

# name of &lt;site&gt;

The name of the site.

# profile of &lt;site&gt;

No documentation exists.

# relevant fixlet of &lt;site&gt;

Iterates through the Relevant Fixlet messages for the specified site.

# relevant offer action of &lt;site&gt;

Returns the list of relevant actions that are offers for the specified site.  This inspector could be useful in a client UI dashboard listing the current set of relevant offers.

# setting &lt;string&gt; of &lt;site&gt;

Returns the setting whose name matches the string provided from the Fixlet site settings.

# setting of &lt;site&gt;

Returns one or more settings from the site settings.

# site tag of &lt;site&gt;

Returns the last component of the specified site&#39;s url, eg. &#39;actionsite&#39;, &#39;enteprisesecurity&#39;, etcetera.

# site version list of &lt;site&gt;

Returns the last gathered site version list (manyversion) of the specified site.

# subscribe time of &lt;site&gt;

Returns the time that the current machine began subscribing to the site.

# type of &lt;site&gt;

Returns one of the following 4 literal strings:Master Action SiteOperator SiteCustom SiteFixlet Site.

# url of &lt;site&gt;

Returns the Locator found in the masthead. A site locator is used to synchronize with the site. It normally contains the URL of a remote file system folder, or the URL of a cgi-bin program that provides a remote directory listing of the site.

# version of &lt;site&gt;

Returns the version number of the site content.
