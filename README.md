# Vidyo Log Viewer

The log viewer assists in debugging client-side issues by grabbing the log from the VidyoClient SDK through a socket and displaying it in a browser with an easy to read format. 

## Usage with VidyoConnector

To use the log viewer with VidyoConnector please follow these steps:

1. Enable Debug in VidyoConnector either through a pull down menu in one of the samples or by calling EnableDebug().
  - EX: in C `VidyoConnectorEnableDebug(c, 7776, "warning all@VidyoClient info@VidyoConnector");`
  - Please take a look at the ReferenceGuide for usage of EnableDebug and possible log filters.
1. Open VidyoLog.html in a browser.
  - By default, the log viewer will query port `7776` on localhost. This is useful for clients running on the same endpoint.
  - To debug a remote endpoint such as iOS or Android device, point to the IP address of the device. EX: `192.168.1.100:7776`
  - Alternatively the contents of the log file such as `VidyoClient.log` can be pasted into `[Paste the log]` section of the header.
  - The `[log filter` dialog allows the log to be filtered for easy viewing. To reset the filter enter an empty string.