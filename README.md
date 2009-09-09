RTFM Money
==========

Decimal types for rails. This is THE LIGHTEST plugin for rails that supports
decimal numeric types in a safe manner.

To install: RTFM
To uninstall: RTFM
To use: RTFM
To profit: RTFM

Clear? Crystal.

Real explanation:
=================

Rails supports a column type :decimal. This uses BigDecimal. It's safe for
calculations - in that it doesn't suffer the classic IEE754 problems with
entropy.

A money plugin for storing a simple numeric type, is completely pointless.
Valid use cases for plugins might include alternative formats for currency
strings not supported by BigDecimal - however, this should not in any way
affect the stored type, or available methods on models. All a good money
plugin should provide is a method for parsing and generating localised money
strings.

Automatic resolution of sub denominal values is also unacceptable, as if
ignored and not correctly accounted for in the business model, this leads to
critical vagueness in applications, and significant money can be lost over
time, or by lawsuit.