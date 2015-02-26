# type: file

For each file in the file system, you can create a corresponding file object and inspect its properties. inspectors are also provided to look at version data of executable files.Note: File systems that do not maintain the creation or last accessed times will often return the last modification time when queried for the creation or last accessed times or files. Modification times are preserved when files are copied. Thus, it is not uncommon to see a file that appears to have been modified before it was created.

# alias of &lt;file&gt;

Returns `True` if the file is an alias for another file.

# aol error of &lt;file&gt;

No documentation exists.

# aol error time of &lt;file&gt;

No documentation exists.

# array of &lt;file&gt;

This inspector creates an OSXArray from the specified XML Data file.

# byte &lt;integer&gt; of &lt;file&gt;

Returns the numeric value of the byte located at the offset specified by number within the file. Byte 0 of the file is the first byte.Example: byte 0 of file &quot;C:\test.txt&quot; - Returns the first byte in the specified file.

# content of &lt;file&gt;

Returns an object that can be used to search for a string in the file. See content.

# creator of &lt;file&gt;

This refers to the four-character identifier used in all MacOS files. The creator tells what application should open the specified file.

# data fork of &lt;file&gt;

Returns information about the data fork of the specified file.

# dictionary of &lt;file&gt;

Returns the dictionary object for the specified file.

# drive of &lt;file&gt;

Returns the drive associated with the specified file. On Macintosh computers, this returns a &lt;volume&gt; object.On  *nix computers, this returns a &lt;filesystem&gt; object.

# executable file format of &lt;file&gt;

Returns a four-byte string containing the format specifier for the specified file.Example: executable file format of client - Returns a string like &quot;PE%00%00&quot;.

# file version of &lt;file&gt;

Returns the file version extracted from the file&#39;s resource block. See version.

# filesystem of &lt;file&gt;

Returns the UNIX filesystem flag for the given file. On a Macintosh, this returns a &lt;volume&gt; object.

# first raw version block of &lt;file&gt;

Returns the first version block directly from a PE file. If the first block is sufficient for your purposes, use this version inspector for best speed.

# json of &lt;file&gt;

No documentation exists.

# key &lt;string&gt; of &lt;file&gt;

Returns a key and its value from the given structured text file. It iterates over lines that start with the key name (as specified by &lt;string&gt;) followed by an = or : character. When searching, white space is ignored.

# length of &lt;file&gt;

The total length of the data and resource forks.Example: Length of data fork of file &quot;Microsoft Word&quot; of folder &quot;Microsoft Office X&quot; of Applications folder is greater than 100000 - Returns `True` if the data fork of the system file is greater than the specified amount.

# line &lt;integer&gt; of &lt;file&gt;

Returns the nth line (specified by &lt;integer&gt;) from the given file.

# line containing &lt;string&gt; of &lt;file&gt;

Returns all lines from the given file that contain the specified string.

# line of &lt;file&gt;

Iterates over all the lines of the specified file. Note that the lines are truncated to 1023 characters.

# line starting with &lt;string&gt; of &lt;file&gt;

Same as line &lt;string&gt; of &lt;file&gt;, returns the lines of the given file that start with the specified string.

# locked of &lt;file&gt;

Returns `True` if the file is locked.Example: locked of file &quot;this file&quot; of folder &quot;this folder&quot; - Returns `True` if the specified file is locked.

# md5 of &lt;file&gt;

Returns the md5 of the file, hex encoded as a string

# only raw version block of &lt;file&gt;

Returns the only version block directly from a PE file.

# only version block of &lt;file&gt;

Most files only have 1 version block. This property allows language independent access when there is only one version block present. The result is the same as &#39;version block 1&#39;.

# pem encoded certificate of &lt;file&gt;

Reads and returns the certificate from a file in the PEM format. This can be used to analyze encryption credentials on decrypting relays or root servers.

# product version of &lt;file&gt;

Returns the product version extracted from the file&#39;s resource block. See version.

# raw file version of &lt;file&gt;

Returns the file version directly from a PE file.

# raw product version of &lt;file&gt;

Returns the product version directly from a PE file.

# raw version block &lt;integer&gt; of &lt;file&gt;

Returns the numbered version block directly from a PE file.

# raw version block &lt;string&gt; of &lt;file&gt;

Returns the named version block directly from a PE file.

# raw version block of &lt;file&gt;

Returns the version block directly from a PE file.

# raw version of &lt;file&gt;

Returns the version directly from a PE file.

# resource fork of &lt;file&gt;

Returns information about the resource fork of the file.

# section &lt;string&gt; of &lt;file&gt;

Returns a named section of a file. Useful for locating sections of &#39;ini&#39; files. Section names are delimited by square bracket characters &#39;[section name]&#39;. See examples below.

# security descriptor of &lt;file&gt;

Specifies the security descriptor associated with the specified file.

# sha1 of &lt;file&gt;

Returns the sha1 checksum of the file hex encoded as a 40 character long string.

# sha224 of &lt;file&gt;

No documentation exists.

# sha256 of &lt;file&gt;

No documentation exists.

# sha2_224 of &lt;file&gt;

Returns the sha2-224 of the file, hex encoded as a string

# sha2_256 of &lt;file&gt;

Returns the sha2-256 of the file, hex encoded as a string

# sha2_384 of &lt;file&gt;

Returns the sha2-384 of the file, hex encoded as a string

# sha2_512 of &lt;file&gt;

Returns the sha2-512 of the file, hex encoded as a string

# sha384 of &lt;file&gt;

No documentation exists.

# sha512 of &lt;file&gt;

No documentation exists.

# shortcut of &lt;file&gt;

Returns the properties and locates the target of a file shortcut:pathname (string)start in pathname (string)argument string (string)icon pathname (string)icon index (integer).

# size of &lt;file&gt;

Returns the size in bytes of a file.

# sqlite database of &lt;file&gt;

No documentation exists.

# stationery of &lt;file&gt;

Returns `True` if the file is a stationery file.

# type of &lt;file&gt;

This refers to the four-character identifier used in all MacOS files. The type describes the sort of file it is.

# variable of &lt;file&gt;

Returns the names of variables contained in an INF style file, in the format [section].name=value.

# version &lt;integer&gt; of &lt;file&gt;

Returns the nth version information from the &quot;vers&quot; resource of the given file. Typically n=1, but other information may be stored in &quot;vers&quot; resources greater than 1.

# version block &lt;integer&gt; of &lt;file&gt;

You can identify the particular version block you want to access by ordinal number.

# version block &lt;string&gt; of &lt;file&gt;

You can identify the particular version block you are looking up by name. The name you provide should match the id string of the version block.

# version block of &lt;file&gt;

Iterates through the version blocks of a file.

# version of &lt;file&gt;

Synonym for file version of &lt;file&gt;.

# visible of &lt;file&gt;

Returns `True` if the file is visible.

# volume of &lt;file&gt;

The volume containing the file.

# windows checksum of &lt;file&gt;

No documentation exists.

# xml document of &lt;file&gt;

Returns an XML Document Object Model (DOM) for the specified file.

# &lt;file&gt; as string

Creates a string containing the full pathname of the specified file. See &lt;file&gt;.
