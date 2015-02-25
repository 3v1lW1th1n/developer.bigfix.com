# statistic range

Statistical ranges are time intervals used to examine particular statistical bins.

# bin at [time] of [statistic range]

Returns the bin in the specified statistical range which brackets the given time. If no such bin exists, it throws NoSuchObject.

# bin of [statistic range]

Returns a list of the individual bins in the specified range. Primarily useful after downsampling (see total &lt;time interval&gt; of &lt;statistic range&gt;).

# end of [statistic range]

Returns the ending time of the statistical range.

# range [time range] of [statistic range]

For the duration of the specified time range, (time0 to time1), this inspector returns a sub-range of bins beginning with earliest bin containing time0 and going up to (but not including) the bin containing time1. If either of these bins does not exist, it throws NoSuchObject.

# start of [statistic range]

Returns the starting time of the statistical range.

# total [time interval] of [statistic range]

This inspector can be used to downsample or consolidate bins. It statistically totals over the given range, producing a new series of bins broken down by the (larger) specified time interval. The resulting range will start and end on a multiple of the interval. For example, if you ask for day bins, the results will start and end at midnight. If the specified time interval is not a multiple of the length of the starting bin of the range, this inspector throws NoSuchObject. For example, you cannot get 6 hour totals of a range which starts with day bins.

# total of [statistic range]

Totals the bins over the specified range, producing a single summary bin. This allows you to reduce the data by constraining the range.
