# type: task principal

The &lt;task principal&lt; inspectors provide information about the scheduled task principal, which incapsulates the security credentials. The principal object includes a display name, a logon type, a run level and a set of IDs.

# display name of &lt;task principal&gt; : string

Returns the name of the principal (as a string) that is displayed in the Task Scheduler UI.

# group id of &lt;task principal&gt; : string

Returns the identifier of the user group (as a string) that is required to run the tasks associated with the principal.

# group logon of &lt;task principal&gt; : boolean

Returns `True` if the task logon type is set to group activation. In this case, the user ID speicifies the group.

# highest runlevel of &lt;task principal&gt; : boolean

Returns `True` if the specfied task principle will be run with the highest privileges.

# id of &lt;task principal&gt; : string

Returns the identifier of the specified task principal as a string type.

# interactive token logon of &lt;task principal&gt; : boolean

Returns `True` if the task logon type is set to interactive token, meaning the task will only run in an existing interactive session.

# interactive token password logon of &lt;task principal&gt; : boolean

Returns `True` if the task logon type is set to interactive token or password. If the user is logged on, the interactive token is used. Otherwise the password is used. The password must have been specified when the task was registered.

# lua runlevel of &lt;task principal&gt; : boolean

Returns `True` if the specfied task principle will be run with the least privileged user account (LUA).

# none logon of &lt;task principal&gt; : boolean

Returns `True` if the logon method for the task principal is not specified. Used for non-NT credentials.

# password logon of &lt;task principal&gt; : boolean

Returns `True` if a password is used for logging on the user. The password must be supplied when the task is registered.

# s4u logon of &lt;task principal&gt; : boolean

Returns `True` if an existing interactive token is used to run the task. This requires the user to employ a service for user (S4U) logon. With S4U logons, no password is stored and neither network nor encrypted files can be accessed.

# service account logon of &lt;task principal&gt; : boolean

Returns `True` if a service account is used as a login. This implies that the task is being initiated by a Local System, Local Service, or Network Service account in a security context.

# user id of &lt;task principal&gt; : string

Returns the user identifier (as a string) required to run the tasks associated with the principal.
