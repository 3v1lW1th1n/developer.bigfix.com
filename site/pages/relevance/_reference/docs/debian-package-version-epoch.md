# type: debian package version epoch

The version string of a Debian package, as displayed by the `dpkg -l` command, follows this format: `[epoch:]upstream_version[-debian_revision]`. Only the `upstream_version` part is required, and the other parts are optional.
See the description of the [debian-package-version](https://developer.bigfix.com/relevance/reference/debian-package-version.html) inspector for more information.

The inspector `debian package version epoch` returns the `epoch` part of the string or an empty string, if that part is absent. The epoch is an unsigned integer, typically a small number. The epoch allows the package provider to create a fresh start with version numbering schemes.

The name structure of Debian package versions is [documented here](https://www.debian.org/doc/debian-policy/ch-controlfields.html#version).

# debian package version epoch &lt;debian package version epoch&gt; : debian package version epoch

A reflexive typing of the specified debian package version epoch.

# extrema of &lt;debian package version epoch&gt; : ( debian package version epoch, debian package version epoch )

Returns the minimum and maximum extreme values of the given list of &lt;debian package version epoch&gt; types.

# maximum of &lt;debian package version epoch&gt; : debian package version epoch

Returns the maximum value from the specified list of Debian package version epochs.

# minimum of &lt;debian package version epoch&gt; : debian package version epoch

Returns the minimum value from the specified list of Debian package version epochs.

# unique value of &lt;debian package version epoch&gt; : debian package version epoch with multiplicity

Returns the unique values and counts of a given list of &lt;debian package version epoch&gt; types, removing duplicates and sorting by value.

# &lt;debian package version epoch&gt; as debian package version epoch : debian package version epoch

Reflexive cast for completeness.

# &lt;debian package version epoch&gt; as string : string

Converts a Debian package version &#39;epoch&#39; into a string.

# &lt;debian package version epoch&gt; &lt; &lt;debian package version epoch&gt; : boolean

No documentation exists.

# &lt;debian package version epoch&gt; &lt;= &lt;debian package version epoch&gt; : boolean

No documentation exists.

# &lt;debian package version epoch&gt; = &lt;debian package version epoch&gt; : boolean

No documentation exists.
