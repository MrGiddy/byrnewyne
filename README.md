fix: Update code for Bokeh 3.0 API changes

Resolved several KeyErrors and AttributeErrors by updating
the plot configuration to be compatible with Bokeh 3.0 and later.

- Replaced `plot_width` and `plot_height` with `width` and `height`.
- Replaced the deprecated `legend` parameter with `legend_label` in glyph methods.
- Corrected the `tools` parameter to accept only a list of tool names,
  adding the configured `HoverTool` object separately using `add_tools()`.
