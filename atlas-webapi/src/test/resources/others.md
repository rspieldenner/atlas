/api/v1/graph?s=e-1d&e=2012-01-01T00:00&q=name,sps,:eq,:sum,(,),:offset,f00,:color
/api/v1/graph?s=e-1d&e=2012-01-01T00:00&q=name,sps,:eq,:sum,(,1d,),:offset,f00,:color
/api/v1/graph?s=e-1d&e=2012-01-01T00:00&q=name,sps,:eq,:sum,2,:lw,(,0h,1d,1w,),:offset,f00,:color
/api/v1/graph?s=e-1d&e=2012-01-01T00:00&q=name,sps,:eq,:sum,2,:lw,(,0h,1d,1w,),:offset,:stack

/api/v1/graph?s=e-1d&e=2012-01-01T00:00&q=42,name,sps,:eq,:sum,(,nf.cluster,),:by,1,:axis
/api/v1/graph?s=e-1d&e=2012-01-01T00:00&q=42,name,sps,:eq,:sum,(,nf.cluster,),:by,1,:axis,37,:area,40,:alpha,2,:axis&u.2=100&l.2=0
/api/v1/graph?s=e-1d&e=2012-01-01T00:00&q=42,name,sps,:eq,:sum,(,nf.cluster,),:by,1,:axis,37,:area,40,:alpha,2,:axis&u.2=100&l.2=0&stack=1
/api/v1/graph?s=e-1d&e=2012-01-01T00:00&q=42,name,sps,:eq,:sum,(,nf.cluster,),:by,1,:axis,37,:area,40,:alpha,2,:axis&u.2=100&l.2=0&stack.1=1
/api/v1/graph?s=e-1d&e=2012-01-01T00:00&q=42,name,sps,:eq,:sum,(,nf.cluster,),:by,1,:axis,f00,:color,37,:area,40,:alpha,2,:axis&u.2=100&l.2=0
/api/v1/graph?s=e-1d&e=2012-01-01T00:00&q=42,name,sps,:eq,:sum,(,nf.cluster,),:by,1w,:offset,1,:axis,37,:area,40,:alpha,2,:axis&u.2=100&l.2=0
/api/v1/graph?s=e-1d&e=2012-01-01T00:00&q=42,name,sps,:eq,:sum,:dup,1w,:offset,1,:axis,:swap,1,:axis,37,:area,40,:alpha,2,:axis&u.2=100&l.2=0
/api/v1/graph?s=e-1d&e=2012-01-01T00:00&q=42,name,sps,:eq,:sum,:dup,1w,:offset,1,:axis,f00,:color,:swap,1,:axis,37,:area,40,:alpha,2,:axis&u.2=100&l.2=0

/api/v1/graph?s=e-1d&e=2012-01-01T00:00&q=name,sps,:eq,:sum,2,:lw,(,0h,1d,1w,),:offset,:stack&zoom=2.0

/api/v1/graph?s=e-1d&e=2012-01-01T00:00&q=42,:area
/api/v1/graph?s=e-1d&e=2012-01-01T00:00&q=42,:area&l=30
/api/v1/graph?s=e-1d&e=2012-01-01T00:00&q=-42,:area
/api/v1/graph?s=e-1d&e=2012-01-01T00:00&q=-42,:area&u=-30

/api/v1/graph?s=e-1d&e=2012-01-01T00:00&q=42,:area,40,:alpha,f00,:color
/api/v1/graph?s=e-1d&e=2012-01-01T00:00&q=42,:area,40,:alpha,ffff0000,:color

/api/v1/graph?s=e-1d&e=2012-01-01T00:00&q=NaN
/api/v1/graph?s=e-1d&e=2012-01-01T00:00&q=NaN,:area
/api/v1/graph?s=e-1d&e=2012-01-01T00:00&q=NaN,:stack,1,:stack

/api/v1/graph?e=2015-05-26T19:52&q=minuteOfHour,:time&s=e-10m

# Make sure significant time boundaries adjust to time zone
/api/v1/graph?q=name,sps,:eq,:sum&s=e-2d&e=2015-06-17T13:13&no_legend=1&tz=US/Pacific
/api/v1/graph?q=name,sps,:eq,:sum&s=e-2d&e=2015-06-17T13:13&no_legend=1&tz=UTC

# Daylight savings time transition
/api/v1/graph?q=name,sps,:eq,:sum&s=e-4d&e=2015-03-10T13:13&no_legend=1&tz=US/Pacific
/api/v1/graph?q=name,sps,:eq,:sum&s=e-4d&e=2015-03-10T13:13&no_legend=1&tz=US/Pacific&step=1d
/api/v1/graph?q=name,sps,:eq,:sum&s=e-4d&e=2015-03-10T13:13&no_legend=1&tz=US/Pacific&tz=UTC
/api/v1/graph?q=name,sps,:eq,:sum&s=e-4d&e=2015-03-10T13:13&no_legend=1&tz=UTC&tz=US/Pacific&tz=US/Eastern&step=1d

# Vision flag
/api/v1/graph?s=e-1d&e=2015-03-10T13:13&q=(,1,2,3,4,5,6,7,8,9,),(,nf.cluster,nccp-silverlight,:eq,name,sps,:eq,:and,:sum,:swap,:legend,),:each&vision=protanopia&no_legend=1&stack=1

# Z-Order of stacked lines
/api/v1/graph?q=t,name,sps,:eq,:sum,:set,t,:get,:stack,t,:get,1.1,:mul,6h,:offset,t,:get,4,:div,:stack&s=e-2d&e=2015-03-10T13:13

# Layout
/api/v1/graph?q=name,sps,:eq,:sum,(,nf.cluster,),:by,:stack&s=e-3h&e=2015-03-10T13:13&w=70&h=70&layout=canvas
/api/v1/graph?q=name,sps,:eq,:sum,(,nf.cluster,),:by,:stack&s=e-3h&e=2015-03-10T13:13&w=70&h=70&layout=image
/api/v1/graph?q=name,sps,:eq,:sum,(,nf.cluster,),:by,:stack&s=e-3h&e=2015-03-10T13:13&w=70&h=70&layout=iw
/api/v1/graph?q=name,sps,:eq,:sum,(,nf.cluster,),:by,:stack&s=e-3h&e=2015-03-10T13:13&w=100&h=70&layout=iw
/api/v1/graph?q=name,sps,:eq,:sum,(,nf.cluster,),:by,:stack&s=e-3h&e=2015-03-10T13:13&w=160&h=70&layout=iw
/api/v1/graph?q=name,sps,:eq,:sum,(,nf.cluster,),:by,:stack&s=e-3h&e=2015-03-10T13:13&w=270&h=70&layout=iw
/api/v1/graph?q=name,sps,:eq,:sum,(,nf.cluster,),:by,:stack&s=e-3h&e=2015-03-10T13:13&w=70&h=70&layout=ih
/api/v1/graph?q=name,sps,:eq,:sum,(,nf.cluster,),:by,:stack&s=e-3h&e=2015-03-10T13:13&w=70&h=7500&layout=iw&title=foo+bar+baz+dlfdkfdsfd

# Axis per line
/api/v1/graph?s=e-1d&e=2012-01-01T00:00&q=name,sps,:eq,:sum,(,nf.cluster,),:by&axis_per_line=1
/api/v1/graph?s=e-1d&e=2012-01-01T00:00&q=name,sps,:eq,:sum,(,nf.node,),:by&axis_per_line=1

# Turning off tick labels
/api/v1/graph?s=e-1d&e=2012-01-01T00:00&q=name,sps,:eq,:sum,(,nf.cluster,),:by&no_tick_labels=1
/api/v1/graph?s=e-1d&e=2012-01-01T00:00&q=42,name,sps,:eq,:sum,(,nf.cluster,),:by,1,:axis&no_tick_labels.1=1
/api/v1/graph?s=e-1d&e=2012-01-01T00:00&q=name,sps,:eq,nf.cluster,nccp-wii,:lt,:and,:sum,(,nf.cluster,),:by&no_tick_labels=1&axis_per_line=1
/api/v1/graph?s=e-1d&e=2012-01-01T00:00&q=name,sps,:eq,nf.cluster,nccp-wii,:lt,:and,:sum,(,nf.cluster,),:by&no_tick_labels.2=1&axis_per_line=1
/api/v1/graph?s=e-1d&e=2012-01-01T00:00&q=name,sps,:eq,nf.cluster,nccp-wii,:lt,:and,:sum,(,nf.cluster,),:by&no_tick_labels.2=1&axis_per_line=1&no_legend_stats=1
