Memory File System
=================
An in memory implementation of a [JSR-203](http://jcp.org/en/jsr/detail?id=203) (Java 7) file system for testing purposes.

Supported
---------
* <code>SeekableByteChannel</code>
* <code>FileChannel</code>
* <code>AsynchronousFileChannel</code>
* <code>UserDefinedFileAttributeView</code>
* <code>InputStream</code>
* <code>OutputStream</code>
* <code>BasicFileAttributeView</code>, <code>BasicFileAttributes</code>
* <code>DosFileAttributeView</code>, <code>DosFileAttributes</code>
* <code>FileOwnerAttributeView</code>
* <code>PosixFileAttributeView</code>, <code>PosixFileAttributes</code>
* <code>UserDefinedFileAttributeView</code>
* <code>FileLock</code>
* <code>PathMatcher</code>
  * glob
  * regex

Not Supported
-------------
* <code>FileChannel#map</code>, </code>MappedByteBuffer<code> has final methods that call native methods
* <code>WatchService</code>
* <code>FileTypeDetector</code>
* cross filesystem copy
* faked DOS view under Linux, totally unspecified
* <code>UnixFileAttributeView</code>, sun package, totally unspecified
* any meaningful access checks