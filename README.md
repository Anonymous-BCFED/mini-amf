> [!IMPORTANT]
> This project is in maintenance mode and will no longer receive major features.
> Issues and feature requests are welcome but are not a priority for me right now.

There are no further planned features.

# Mini-AMF

Mini-AMF provides Action Message Format
([AMF](https://en.wikipedia.org/wiki/Action_Message_Format))
serialization and deserialization support for
[Python](https://www.python.org), compatible with the [Adobe Flash
Player](https://en.wikipedia.org/wiki/Flash_Player). It supports Python
2.7 and 3.4+.

Mini-AMF is a trimmed-down version of the [original
PyAMF](https://github.com/hydralabs/pyamf), which (as far as I can tell)
is no longer being maintained. It provides only the core serialization
and deserialization primitives, and support for reading and writing
[LSO](https://en.wikipedia.org/wiki/Local_shared_object) objects on
disk. Support for Flex-specific types, \"remoting\", and integration
with web frameworks has all been removed. (Adapter classes are still
supported.)

Mini-AMF is lightly maintained by ~~[Zack
Weinberg](https://www.owlfolio.org/)~~ Anonymous-BCFED. All bug reports and pull requests
will be heard and responded to, but I have no plans to develop the
software any further myself. Please also note that "remoting" and server
integration will probably be easier to maintain in their own separate
packages, one per framework.

## What's AMF?

AMF is a binary message serialization format geared for remote procedure
calls, native to the [Adobe Flash
Player](https://en.wikipedia.org/wiki/Flash_Player) and [Adobe
Integrated Runtime](https://en.wikipedia.org/wiki/Adobe_AIR). There are
two versions of the format, AMF0 and AMF3. AMF3 is more compact than
AMF0, and and supports data types that are available only in
[ActionScript](https://en.wikipedia.org/wiki/ActionScript) 3.0, such as
ByteArray.
