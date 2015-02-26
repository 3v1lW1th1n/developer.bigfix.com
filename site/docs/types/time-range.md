# type: time range

The &lt;time range&gt; inspectors provide tools for dealing and calculating with time-range types, which are of the form &#39;time to time&#39;, such as Tue, 18 Apr 2006 16:46:07 -0400 to Wed, 19 Apr 2006 16:46:07 -0400

# end of &lt;time range&gt;

Returns the end date of a time range.

# final part &lt;time interval&gt; of &lt;time range&gt;

Returns a time range with the specified interval, but ending on the final date of the time range.

# initial part &lt;time interval&gt; of &lt;time range&gt;

Returns a time range starting with the first date of the time range and lasting for the specified interval.

# length of &lt;time range&gt;

Returns the time interval (in days, hours, minutes, seconds) between the start and end date of a time range.

# range after &lt;time&gt; of &lt;time range&gt;

Returns a new time range, starting from the specified time and continuing through the end of the original range. The time must be within the range, or an error will result.

# range before &lt;time&gt; of &lt;time range&gt;

Returns a new time range, starting from the original time in the specified range and continuting to the specified time. The time must be within the range, or an error will result.

# start of &lt;time range&gt;

Returns the starting date of a time range.

# unique value of &lt;time range&gt;

Returns the unique values of a given list of &lt;time range&gt; types, removing duplicates and sorting by value.

# &lt;time range&gt; as string

Casts a time range as a string.
