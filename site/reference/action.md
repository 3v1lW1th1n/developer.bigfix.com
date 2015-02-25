# action

The &lt;action&gt; objects are the keywords associated with properties available for inspection during the execution of BigFix Actions.

# active count of [action]

No documentation exists.

# active line number of [action]

No documentation exists.

# active of [action]

Returns `True` if the action is currently running (active).

# active start time of [action]

Returns the time the action started.

# complete time of [action]

Returns the time the action completed.

# constrained of [action]

Returns `True` if action is unable to run yet.

# constraint of [action]

No documentation exists.

# download failure of [action]

No documentation exists.

# exit code of [action]

Returns an integer corresponding to the exit code of the specified action. This value will not exist if the action has not yet produced an exit code.

# first active count of [action]

No documentation exists.

# group leader of [action]

Returns `True` if the action is a group action and the action component is the group leader. When you deploy a mult-action from the BES Console, it constructs a group action with a group leader to control the overall behavior of the action. This inspector is used internally to manage the progress of the group action.

# header [string] of [action]

No documentation exists.

# header of [action]

No documentation exists.

# id of [action]

Returns the numeric ID associated with the specified Action.

# last active line number of [action]

No documentation exists.

# last active time of [action]

No documentation exists.

# last change time of [action]

Returns the time when the action state last changed.

# offer accepted of [action]

Returns `True` when users indicated they want to run the action by accepting the offer presented by the BES Client UI. When an offer has been accepted, the Client evaluates its constraints and runs as soon as conditions allow.

# offer of [action]

Returns `True` when the Action is presented as an offer (as indicated by the header &quot;x-offer: 1&quot;).

# origin fixlet id of [action]

Returns the Fixlet id that contained the action.

# parameter [string] of [action]

Returns the value of parameter &lt;string&gt; for the active Action. Parameters only live as long as the action is active. Among the inspectable parameters is the &#39;action issue date&#39; that is added to each Action by the BigFix Console at issue time.Example: parameter &quot;action issue date&quot; of action - This inspector returns the date the action was issued, a parameter added to each action by the BigFix Console.

# pending login of [action]

Returns `True` if the specified action included an &#39;action requires login&#39; command, and a login has not yet occurred since the action has run.

# pending of [action]

Returns `True` if action is available to run.

# pending restart of [action]

Returns `True` if the specified action included an &#39;action requires restart&#39; command and a restart has not occurred since the action has run.

# pending time of [action]

Returns the time the action became pending.

# persistent constraint of [action]

No documentation exists.

# status of [action]

Returns one of the following strings: Running = when the action is currently active. Executed = no longer relevant and action has completed. Not Relevant = action was not relevant. Waiting = action is relevant, but waiting to run. Not Executed = action is relevant, unconstrained, but has not yet started. Failed = action is relevant, unconstrained, has completed, but is still relevant.

# system constraint of [action]

No documentation exists.

# waiting for download of [action]

Returns `True` if client is waiting for mirroring server to have downloads required by the action.

# [action] as string

No documentation exists.
