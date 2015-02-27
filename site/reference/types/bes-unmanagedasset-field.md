# type: bes unmanagedasset field

The &lt;bes unmanagedasset field&gt; inspectors provide authors with access to the individual fields of various unmanaged assets. Each field consists of a name / value pair, analogous to BES properties. There are three types of fields:IdentifyingField: Each asset must have one IdentifyingField, such as a MAC Address, which is used to identify and correlate different reports from the same asset.FilterableField: These are displayed in the Console in both the Unmanaged Asset list and the unmanaged asset document, allowing sorting and filtering.NonFilterable: These are only displayed in the Unmanaged Assets document, and typically return a large amount of data, such as a list of vulnerabilities.

# asset of &lt;bes unmanagedasset field&gt;

Returns an asset (containing a name / value pair) from the specified BES unmanaged asset field.

# editable flag of &lt;bes unmanagedasset field&gt;

Returns `True` if the specified BES Unmanaged Asset is editable.

# filterable flag of &lt;bes unmanagedasset field&gt;

Returns `True` if the specified asset field is filterable. Fields that are filterable will show up in the Unmanaged Assets list, allowing you to sort and filter them.

# name of &lt;bes unmanagedasset field&gt;

Returns the name of the specified BES unmanaged asset field.

# value of &lt;bes unmanagedasset field&gt;

Returns the value (as a &lt;string&gt;) of the specified BES Unmanaged Asset field.
