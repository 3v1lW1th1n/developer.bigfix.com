# type: distinguished name

The `distinguished name` type represents an Active Directory or LDAP distinguished name.

# component &lt;integer&gt; of &lt;distinguished name&gt; : distinguished name component

Returns the nth component of the distinguished name.

{{#example}}
Q: component 1 of distinguished name &quot;CN=bearmo,OU=bears,DC=example,DC=com&quot;
A: OU=bears
{{/example}}

# component of &lt;distinguished name&gt; : distinguished name component

Returns a list of the components of the distinguished name.

{{#example}}
Q: components of distinguished name &quot;CN=bearmo,OU=bears,DC=example,DC=com&quot;
A: CN=bearmo
A: OU=bears
A: DC=example
A: DC=com
{{/example}}
