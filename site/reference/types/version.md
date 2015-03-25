# type: version

This is the numeric method of indicating the file version, which is compact, convenient and fast. It makes use of a short string to define the version number. Version types are available as both client and core inspectors, so if you don&amp;#39;t find what you want in one guide, please check the other.

# bug revision of &lt;version&gt; : integer

If the stage is present the bug revision is the number after the stage. If absent, zero is implied.

# build revision of &lt;version&gt; : integer

Returns the final component of a version (Major.Minor.RevisionStageBuild).Example: build revision of version &amp;quot;7.1.2.70&amp;quot; - Returns 70.

# extrema of &lt;version&gt; : ( version, version )

Returns the minimum and maximum extreme values of the given list of &amp;lt;version&amp;gt; types.

# major revision of &lt;version&gt; : integer

The number before the first period in the version string.Example: major revision of version of file &amp;quot;name&amp;quot; &amp;gt; 4 - Returns `True` if the major revision number is greater than the specified number.

# maximum of &lt;version&gt; : version

Returns the maximum value from a list of &amp;lt;version&amp;gt; types.

# minimum of &lt;version&gt; : version

Returns the minimum value from a list of &amp;lt;version&amp;gt; types.

# minor revision of &lt;version&gt; : integer

The number immediately after the first period in the version string. If absent, zero is implied.

# pad of &lt;version&gt; : version

Returns a version object which is padded with zero values.

# stage of &lt;version&gt; : stage

The stage is represented by the letter in the version string. It may be &amp;#39;a&amp;#39; for alpha, &amp;#39;b&amp;#39; for beta, &amp;#39;d&amp;#39; for development or &amp;#39;f&amp;#39; for final. If absent, final is implied.

# unique value of &lt;version&gt; : version with multiplicity

Returns the unique values of a given list of &amp;lt;version&amp;gt; types, removing duplicates and sorting by value.

# &lt;version&gt; as string : string

Turns a version type into a string of the form &amp;quot;1.2.3.4&amp;quot;.Example: version of regapp &amp;quot;bigfix.exe&amp;quot; as string = &amp;quot;1.0.45.0&amp;quot; - Returns `True` if the BigFix application has the specified version.Example: version of package &amp;quot;BESAgent&amp;quot; of rpm as string = &amp;quot;3.1.0.19-1&amp;quot; - TRUE if the BESAgent program has the given version.

# &lt;version&gt; as version : version

Reflexive cast of version.

# &lt;version&gt; &lt; &lt;version&gt; : boolean

No documentation exists.

# &lt;version&gt; &lt;= &lt;version&gt; : boolean

No documentation exists.

# &lt;version&gt; = &lt;version&gt; : boolean

No documentation exists.
