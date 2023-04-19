# floating-monitor
A floating monitor window(Based on pyqt5) to show net speed,cpu load and memory use.

### monitor.py
	The original script, import ui window from monitor_ui.py, no qtsignal was used.
### monitor_ui.pu
	Script generated from monitor.ui.
### <font color=green>monitor_Qthread.py</font>
	The most stable and resource saving version;It's recommand to use this one.
### monitor_Threading.py
	Use threading module to get computer info, another way to realize function.

## Picture
![avatar](data:image/png;base64,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)