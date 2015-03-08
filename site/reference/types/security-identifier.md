# type: security identifier

A Security Identifier, or SID, is a data structure that identifies user, group, and computer accounts. Every account on a network is issued a unique SID when the account is first created. Internal processes in Windows refer to an account&#39;s SID rather than the account&#39;s user or group name.

# account name of &lt;security identifier&gt;

Retrieves the name of the account for this SID and the name of the first domain on which this SID is found.

# component string of &lt;security identifier&gt;

This inspector returns a string formatted using the [ConvertSidToStringSid](https://msdn.microsoft.com/en-us/library/windows/desktop/aa376399%28v=vs.85%29.aspx) function.

{{#example}}
Q: component string of owner of security descriptor of windows folder
A: S-1-5-80-956008885-3418522649-1831038044-1853292631-2271478464
I: singular string
{{/example}}

# domain name of &lt;security identifier&gt;

Returns the domain name of the first domain on which the specified SID is found.

# rsop user wmi &lt;security identifier&gt;

Each user has its own RSoP (Resultant Set of Policy) namespace based on the user&#39;s Security Identifier (SID). This inspector returns the namespace specified by the &lt;security identifier&gt;.

# user of &lt;security identifier&gt;

No documentation exists.

# &lt;security identifier&gt; as string

Returns the security identifier in string format.

# &lt;security identifier&gt; = &lt;security identifier&gt;

Tests two &lt;security identifier&gt; (SID) values for equality using EqualSid.
