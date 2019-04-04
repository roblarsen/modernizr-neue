## Deprecated Feature Tests

The following tests have been removed from Modernizr.

### touch/touchevents

This test has been preblematic for many years. Originally named `touch` the assumption was that it indicated whether or not the device in question had touch capability. This is not what the test does. The basic test, `if (ontouchstart in window)`, checks to see if the browser supports touch events as a browser feature and doesn't inform the user anything at all about the capabilities of the device.

The test was renamed `touchevents` to more accurately describe the test, but that didn't improve understanding of what the test actually indicated.

This confusion is compounded by the fact that there is no way to definitively test for touch capabilities.