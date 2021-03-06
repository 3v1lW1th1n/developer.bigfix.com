# type: rpm package version

The &lt;rpm package version&gt; inspectors disclose properties of the RPM package version record inspector. They are collected from the 'Version' component of the Epoch, Version and Release fields associated with an RPM package. The behavior of this inspector differs from a string, because they are sorted according to RPM rules defined by the `rpmvercmp()` function of the RPM library. Do not create an &lt;rpm package release&gt; inspector with embedded '-' or whitespace characters. These characters are disallowed in RPM, and will cause the statement to fail.

**Note**: Requires the presence of the RPM library and `librpminfo` (an open source library created by BigFix containing modified RPM library code) on the client machine. `librpminfo` is installed on the client as part of the normal BES client RPM installation procedure.

# extrema of &lt;rpm package version&gt; : ( rpm package version, rpm package version )

Returns the minimum and maximum extreme values of the given list of RPM package versions.

# maximum of &lt;rpm package version&gt; : rpm package version

Returns the maximum value from a list of &lt;rpm package version&gt; types.

# minimum of &lt;rpm package version&gt; : rpm package version

Returns the minimum value from a list of &lt;rpm package version&gt; types.

# rpm package version &lt;rpm package version&gt; : rpm package version

Iterates through the RPM package version objects.

# unique value of &lt;rpm package version&gt; : rpm package version with multiplicity

Returns the unique values of a given list of &lt;rpm package version&gt; types, removing duplicates and sorting by value.

# &lt;rpm package version&gt; as rpm package version : rpm package version

No documentation exists.

# &lt;rpm package version&gt; as string : string

Casts an RPM package version as a string type.

# &lt;rpm package version&gt; &lt; &lt;rpm package version&gt; : boolean

No documentation exists.

# &lt;rpm package version&gt; &lt;= &lt;rpm package version&gt; : boolean

No documentation exists.

# &lt;rpm package version&gt; = &lt;rpm package version&gt; : boolean

No documentation exists.
