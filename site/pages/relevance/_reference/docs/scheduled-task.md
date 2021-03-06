# type: scheduled task

The &lt;scheduled task&gt; inspectors are built on top of the Windows Task Scheduler (see the MSDN reference). There are two versions: the 1.0 interface (Win 2000, XP &amp; Server 2003) and the 2.0 interface (Win 7, Vista and Server 2008) which is favored when available. The Task Scheduler inspector set reflects the 2.0 interface layout which in turn maps back to the 1.0 interface. Features of the 1.0 interface are available in the 2.0 interface, but not vice-versa. If the 2.0 interface isn&#39;t available, you may encounter undefined objects. Each of these inspectors works with both 1.0 and 2.0 unless explicitly Noted.

# definition of &lt;scheduled task&gt; : task definition

Returns the task definition for the specified scheduled task for both the 1.0 and 2.0 interface.

# disabled state of &lt;scheduled task&gt; : boolean

Returns a boolean indicating the whether the specified task is disabled or not.

# enabled of &lt;scheduled task&gt; : boolean

Returns a boolean TRUE if the specified scheduled task is enabled.

# last run time of &lt;scheduled task&gt; : time

Returns the time corresponding to when the specified scheduled task was last run.

# last task result of &lt;scheduled task&gt; : integer

Returns an integer corresponding to the last result of the specified scheduled task.

# missed run count of &lt;scheduled task&gt; : integer

Returns an integer corresponding to the missed run count of the specified scheduled task.

# name of &lt;scheduled task&gt; : string

Returns the name of the specified scheduled task.

# next run time of &lt;scheduled task&gt; : time

Returns the next time that the specified task is scheduled to run.

# path of &lt;scheduled task&gt; : string

Returns the path of the specified scheduled task.2.0 interface only.

# queued state of &lt;scheduled task&gt; : boolean

Returns a boolean indicating the whether the specified task is queued or not.

# ready state of &lt;scheduled task&gt; : boolean

Returns a boolean indicating the whether the specified task is ready or not.

# running state of &lt;scheduled task&gt; : boolean

Returns a boolean indicating the whether the specified task is running or not.

# security descriptor of &lt;scheduled task&gt; : security descriptor

Returns the security descriptor for the specified scheduled task.2.0 interface only.

# trigger string of &lt;scheduled task&gt; : string

Returns the triggering string for the specified scheduled task.1.0 interface only.

# unknown state of &lt;scheduled task&gt; : boolean

Returns `True` if the state of the scheduled task is unknown.2.0 interface only.

# xml of &lt;scheduled task&gt; : string

Returns a string containing the XML content of the specified scheduled task. 2.0 interface only.
