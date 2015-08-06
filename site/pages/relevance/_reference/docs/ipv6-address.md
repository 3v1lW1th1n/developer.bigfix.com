# type: ipv6 address

The &lt;ipv6 address&gt; inspectors deal with the Internet Protocol addressing scheme, version 6. Note: Prior to version 8.0 of BigFix, this was not a derived type.

# extrema of &lt;ipv6 address&gt; : ( ipv6 address, ipv6 address )

Returns the minimum and maximum extreme values of the given list of &lt;ipv6 address&gt; types.

# hexadecet &lt;integer&gt; of &lt;ipv6 address&gt; : integer

Returns one of the eight 16-bit parts (hexadecets) of an IPv6 address specified by &lt;integer&gt;. Here zero refers to the highest hexadecet (network or big-endian order). Thus hexadecet 0 refers to the most-significant 16-bits of the 128 bit IPv6 address.

# ipv4 part of &lt;ipv6 address&gt; : ipv4 address

Returns the lowest 32-bits of the IPv6 address as an IPv4 address.As of version 8.0, this inspector type is derived from an &lt;ipv4or6 address&gt; type.

# maximum of &lt;ipv6 address&gt; : ipv6 address

Returns the maximum value from a list of &lt;ipv6 address&gt; types.

# minimum of &lt;ipv6 address&gt; : ipv6 address

Returns the minimum value from a list of &lt;ipv6 address&gt; types.

# unique value of &lt;ipv6 address&gt; : ipv6 address with multiplicity

Returns the unique values of a given list of &lt;ipv6 address&gt; types, removing duplicates and sorting by value.

# &lt;ipv6 address&gt; as compressed string : string

Similar to casting as a string, but with double colons used to represent multiple zero 16-bit parts (RFC 4291 section 2.2, item 2).

# &lt;ipv6 address&gt; as compressed string with ipv4 : string

Similar to casting as a string, but with both colon-compression and standard IPv4 representation for the low 32-bits.

# &lt;ipv6 address&gt; as compressed string with ipv4 with zone index : string

Similar to casting as a string, but with both colon-compression and standard IPv4 representation for the low 32-bits as well as any zone index.

# &lt;ipv6 address&gt; as compressed string with zone index : string

Similar to casting as a string, but with both colon-compression and a zone index.

# &lt;ipv6 address&gt; as ipv4or6 address : ipv4or6 address

Casts an IPv6 address as a more flexible ipv4or6 address.

# &lt;ipv6 address&gt; as string : string

Returns a string representation of the IPv6 address in the form x:x:x:x:x:x:x:x, where each x represents one to four hexadecimal digits of the eight 16-bit address fields. Leading zeros in an individual field are omitted. See RFC 4291 section 2.2, item 1.

# &lt;ipv6 address&gt; as string with ipv4 : string

Similar to casting as a string, but with the lowest 32 bits of the address in the standard IPv4 representation (RFC 4291 section 2.2, item 3).

# &lt;ipv6 address&gt; as string with ipv4 with zone index : string

Similar to casting as a string, but with standard IPv4 representation for the low 32-bits as well as any zone index.

# &lt;ipv6 address&gt; as string with leading zeros : string

Similar to casting as a string, but leading zeros in individual fields are preserved.

# &lt;ipv6 address&gt; as string with leading zeros with zone index : string

Converts an IPv6 address into a string with all fields packed with leading zeroes as well as a terminating zone index, if any.

# &lt;ipv6 address&gt; as string with zone index : string

Converts an IPv6 address into a string with a terminating slash-delimited zone index, if any.

# &lt;ipv6 address&gt; &lt; &lt;ipv6 address&gt; : boolean

No documentation exists.

# &lt;ipv6 address&gt; &lt;= &lt;ipv6 address&gt; : boolean

No documentation exists.

# &lt;ipv6 address&gt; = &lt;ipv6 address&gt; : boolean

No documentation exists.
