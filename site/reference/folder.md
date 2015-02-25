# folder

For every folder that exists in the file system, you can create a folder object. These inspectors allow you to examine dozens of properties of folder objects. On the Macintosh, there are dozens of specialized folders; access to them depends on the domain. If the domain is not specified, it defaults to the system domain.

# application [string] of [folder]

Returns an application object for the named file located in the folder. See application.Example: exists application &quot;notepad.exe&quot; of the windows folder - Using the application of folder creation method, this example locates the notepad application provided it exists in the Windows folder.

# application of [folder]

Recursively finds executables in the supplied folder, returning a list of &quot;application&quot; objects, which are basically  filesystem_objects.Example: applications of folder &quot;/Users/fizzle/bin&quot; - Returns a list of applications in the specified directory, such as /Users/fizzle/bin/p4, /Users/fizzle/bin/mylocaltool.

# bundle of [folder]

Returns a bundle from a folder (if it has one like application folders do).Example: exists (bundle of applications folder) - Typically returns `True`.

# bundle version of [folder]

Returns the version of the folder corresponding to the CFBundleVersion string, as distinct from the CFBundleShortVersionString.

# descendant folder of [folder]

Returns the descendant folders, recursively, of the given folder. The folder equivalent of &quot;descendants of &lt;folder&gt;&quot;.

# descendant of [folder]

Returns a list of all the descendant files of the specified folder.

# device file [string] of [folder]

Returns the device file with the specified name in the given folder.

# device file of [folder]

Returns the device files that exist in the specified folder.

# drive of [folder]

Returns the drive associated with the specified folder.On Macintosh computers, this returns a &lt;volume&gt; object.On  *nix computers, this returns a &lt;filesystem&gt; object.

# fifo file [string] of [folder]

Returns the FIFO file (named pipe) with the given name in the specified folder.

# fifo file of [folder]

Returns the list of FIFO file in the given folder.

# file [string] of [folder]

Returns a file object for the named file located in the folder.Example: exists file whose (name of it contains &quot;.pdf&quot;) of folder &quot;name&quot; - Returns `True` if some file in the folder has a name including the string &quot;.pdf&quot;.

# file ending in [string] of [folder]

Returns a list of files ending in &quot;xxxx&quot;. Typically used to identify a dotted extension. Equivalent to a wildcard search for &quot;*xxxx&quot;.Example: files ending in &quot;.a&quot; of folder &quot;/usr/lib&quot;  - Returns a list of files with the specified ending, such as: /usr/lib/libcpp_kext.a, /usr/lib/libfl.a, /usr/lib/libioabc.a, and others.

# file of [folder]

Iterates through the files of a folder returning file objects. When combined with a whose clause you can select files with specific properties. See file.

# filesystem of [folder]

Returns the filesystem on which the folder resides. On a Macintosh, this inspector returns a &lt;volume&gt; object.

# find file [string] of [folder]

Iterates through the files of a folder returning file objects whose name matches the wildcard string provided in the name parameter.  A wildcard string uses an asterisk to stand for any number of characters (incuding zero), and a question mark to stand for exactly one character. Thus A??.txt would match All.txt and AXE.txt but not all.txt or a.txt. See example below.Example: Number of find files &quot;siteico*.bmp&quot; of client folder of current site = 3 - Returns `True` if there are 3 files matching the wildcard pattern siteico*.bmp.Example: names of find files &quot;*.exe&quot; of windows folder - Returns a list of the names of all the executable programs in the Windows folder.

# find folder [string] of [folder]

Finds the folder with the given wildcard name inside another folder. A wildcard string uses an asterisk to stand for any number of characters (incuding zero), and a question mark to stand for exactly one character. Thus A??.txt would match All.txt and AXE.txt but not all.txt or a.txt.

# find item [string] of [folder]

Returns the filesystem objects matching the item wildcard string of the given folder. Macintosh &#39;items&#39; are analogous to files and folders on other systems. A wildcard string uses an asterisk to stand for any number of characters (incuding zero), and a question mark to stand for exactly one character. Thus A??.txt would match All.txt and AXE.txt but not all.txt or a.txt.

# folder [string] of [folder]

Returns a folder object for the named sub-folder. Trailing slashes should be omitted from the name.

# folder ending in [string] of [folder]

Returns a list of folders ending in &quot;xxxx&quot;. Typically used to identify a dotted extension. Equivalent to a wildcard search for &quot;*xxxx&quot;.

# folder of [folder]

Iterates through the folders of a folder returning folder objects. When combined with a whose clause, you can select folders with specific properties.

# hfs relative item [string] of [folder]

Returns a filesystem object with the given wildcard name from the specified folder, using HFS format. A wildcard string uses an asterisk to stand for any number of characters (incuding zero), and a question mark to stand for exactly one character. Thus A??.txt would match All.txt and AXE.txt but not all.txt or a.txt.

# item [string] of [folder]

Returns the named item (file or folder) from the specified folder.

# item ending in [string] of [folder]

Returns a list of items (files/folders) ending in &quot;xxxx&quot;. Typically used to identify a dotted extension. Equivalent to a wildcard search for &quot;*xxxx&quot;.

# item of [folder]

Returns a list of the items (file or folder) in the specified folder.Example: names of items of applications folder - Returns a list of applications, such as DS_Store, .localized, AddressBook.app, AppleScript, Calculator.app, Chess.app, DVD Player.app, etc....

# posix relative item [string] of [folder]

Returns a filesystem object with the given relative item name from the specified folder, using POSIX format.

# relative file [string] of [folder]

Returns the file with the path specified by &lt;string&gt; relative to the given &lt;folder&gt;.Example: relative file &quot;Safari.app/Contents/MacOS/Safari&quot; of applications folder - Returns the concatenation of the specified folder and the given path, /Applications/Safari.app/Contents/MacOS/Safari.

# relative folder [string] of [folder]

Returns the folder with the path specified by &lt;string&gt; relative to the given &lt;folder&gt;.

# relative hfs file [string] of [folder]

Returns the HFS file with the path specified by &lt;string&gt; relative to the given &lt;folder&gt;.

# relative hfs folder [string] of [folder]

Returns the HFS folder with the path specified by &lt;string&gt; relative to the given &lt;folder&gt;.

# relative item [string] of [folder]

Returns a filesystem object with the given relative item name from the specified folder, using POSIX format.

# relative posix file [string] of [folder]

Returns the POSIX file with the path specified by &lt;string&gt; relative to the given &lt;folder&gt;.

# relative posix folder [string] of [folder]

Returns the POSIX folder with the path specified by &lt;string&gt; relative to the given &lt;folder&gt;.

# security descriptor of [folder]

Specifies the security descriptor associated with the specified folder.

# socket file [string] of [folder]

Returns the socket file with the given name in the specified folder.

# socket file of [folder]

Returns the socket file(s) in the specified folder.

# symlink [string] of [folder]

Returns the named symlink from the specified folder.

# symlink of [folder]

Returns the symlink(s) in the specified folder, whether or not they are broken. Note: This behavior differs from looking for files in a folder. Although that returns links along with the files, it doesn&#39;t return broken links.

# version of [folder]

Returns a version for a folder representing an application.

# volume of [folder]

The volume containing the specified folder.
