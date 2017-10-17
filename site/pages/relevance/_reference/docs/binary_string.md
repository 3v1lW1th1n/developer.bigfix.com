# type: binary_string

Creates a binary string from the hexadecimal notation. The string must contain only the characters 0-9 and a-f. For example:

{% qna %}
Q: binary_string "82a4"
{% endqna %}

returns binary string of 2 bytes, the first byte contains 0x82, second byte contains 0xa4.

# application &lt;binary_string&gt; : application

Returns the named applications (bundles) and executables as binary filesystem objects.

# binary_substring &lt;( integer, integer )&gt; of &lt;binary_string&gt; : binary_substring

Returns binary_substring containing length `integer` bytes from position `integer`. Position is zero origin.

{% qna %}
Q: (binary_substring(2,3) of (binary_string "001122334455667788")) as hexadecimal
A: 223344
{% endqna %}

{% qna %}
Q: binary_substrings (integers in (0, length of it, 1), 1) of binary_string "68656c6c6f2f776f726c64"
A: h
A: e
A: l
A: l
A: o
A: /
A: w
A: o
A: r
A: l
A: d
{% endqna %}

# binary_substring &lt;binary_string&gt; of &lt;binary_string&gt; : binary_substring

Iterates through the binary string returning all the binary substrings matching the name given.

{% qna %}
Q: number of binary_substrings (binary_string "11") of (binary_string "11225511225511")
A: 3
{% endqna %}

# byte &lt;integer&gt; of &lt;binary_string&gt; : binary_substring

Returns the binary substring value of the byte located at the offset specified by number. Number is zero origin.  

{% qna %}
Q: (byte 0 of (binary_string "1122334455")) as hexadecimal 
A: 11
{% endqna %}

# byte of &lt;binary_string&gt; : binary_substring

Returns each byte of `binary_string` as separate data. 

{% qna %}
Q: (bytes of (binary_string "1122ee33ff")) as hexadecimal
A: 11
A: 22
A: ee
A: 33
A: ff
{% endqna %}

# file &lt;binary_string&gt; : file

Returns a file object for the binary name provided.

# first &lt;integer&gt; of &lt;binary_string&gt; : binary_substring

Returns a binary substring containing first `integer` bytes of `binary_string`.

{% qna %}
Q: first 3 of (binary_string "112233445566778899") as hexadecimal  
A: 112233
{% endqna %}

{% qna %}
Q: first 5 of "To be or not to be"  
A: To be
{% endqna %}

# folder &lt;binary_string&gt; : folder

Returns a folder object for the binary name provided.

# last &lt;integer&gt; of &lt;binary_string&gt; : binary_substring

Returns a binary substring containing last `integer` bytes of `binary_string`.

{% qna %}
Q: (last 2 of (binary_string "112233445566778899")) as hexadecimal
A: 8899
{% endqna %}

# length of &lt;binary_string&gt; : integer

Returns the length of the binary string in number of bytes.

# percent encode &lt;binary_string&gt; : string

Provides percent encoded format of binary data of `binary_string`. 

{% qna %}
Q: percent encode (binary_string "003182")  
A: %25001%2582
{% endqna %}

# position &lt;integer&gt; of &lt;binary_string&gt; : binary position

Returns the position of a binary string.

# position of &lt;binary_string&gt; : binary position

Returns the binary positions of the binary string.

# representable in &lt;string&gt; of &lt;binary_string&gt; : boolean

Checks if the binary value in the binary string is valid in one or more encodings.
To specify multiple encodings, separate them with a semicolon. The binary value is tested with the first encoding, and if it is not valid, it is tested against next encoding until a valid encoding, among those specified, if found or untile the list of encodings to test ends. The inspector returns true if binary value is valid in any of specified encodings, returns false otherwise.

{% qna %}
Q: representable in "UTF-8;Shift_JIS" of (binary_string "82a082a2")  
A: True
{% endqna %}

# representable in utf16 of &lt;binary_string&gt; : boolean

Returns true if binary data in `binary_string` is valid UTF-16 data.

# representable in utf8 of &lt;binary_string&gt; : boolean

Returns true if binary data in `binary_string` is valid UTF-8 data.

# representable of &lt;binary_string&gt; : boolean

Returns true if binary data in `binary_string` is valid UTF-16 data on Windows systems. Returns true if binary data in `binary_string` is valid UTF-8 data on non-Windows systems.

# representation in &lt;string&gt; of &lt;binary_string&gt; : string

Tries to transcode binary data in `binary_string` from the specified encoding to UTF-8. If the conversion succeeds, returns the converted data, if the conversion does not succeed, tries next encodings.

{% qna %}
Q: representations in "UTF-8;euc_jp;Shift_JIS" of (binary_string "e3838fe383ad")
A: "ハロ"
{% endqna %}

# symlink &lt;binary_string&gt; : symlink

Returns a symbolic link from the specified binary string.

# uuid &lt;binary_string&gt; : uuid

No documentation exists.

# &lt;binary_string&gt; as fxf string : string

Interprets binary data in `binary_string` as fxf character set and converts to string.

# &lt;binary_string&gt; as hexadecimal : string

Converts a binary string to a hexadecimal number.

# &lt;binary_string&gt; as local string : string

Interprets binary data in `binary_string` as local character set and converts to string.

# &lt;binary_string&gt; as string : string

Interprets binary data in binary_string as UTF-16 and converts to string on Windows systems. Interprets binary data in binary_string as UTF-8 and converts to string on non-Windows systems.

# &lt;binary_string&gt; as utf16 string : string

Interprets binary data in `binary_string` as UTF-16 and converts to string.

# &lt;binary_string&gt; as utf8 string : string

Interprets binary data in `binary_string` as UTF-8 and converts to string.

# &lt;binary_string&gt; &amp; &lt;binary_string&gt; : binary_string

No documentation exists.

# &lt;binary_string&gt; &lt; &lt;binary_string&gt; : boolean

No documentation exists.

# &lt;binary_string&gt; &lt;= &lt;binary_string&gt; : boolean

No documentation exists.

# &lt;binary_string&gt; = &lt;binary_string&gt; : boolean

No documentation exists.

# &lt;binary_string&gt; contains &lt;binary_string&gt; : boolean

Returns a boolean TRUE if the first `binary_string` contains with the second `binary_string`. The value is checked on byte basis.

{% qna %}
Q: (binary_string "11ee22") contains (binary_string "ee") 
A: True
{% endqna %}

{% qna %}
Q: (binary_string "11ee22") contains (binary_string "1e") 
A: False
{% endqna %}

# &lt;binary_string&gt; ends with &lt;binary_string&gt; : boolean

Returns a boolean TRUE if the first `binary_string` ends with the second `binary_string`.

# &lt;binary_string&gt; starts with &lt;binary_string&gt; : boolean

Returns a boolean TRUE if the first `binary_string` starts with the second `binary_string`.
