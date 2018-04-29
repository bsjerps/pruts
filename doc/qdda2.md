Content-type: text/html; charset=UTF-8

<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN">
<HTML><HEAD><TITLE>Man page of qdda</TITLE>
</HEAD><BODY>
<H1>qdda</H1>
Section: QDDA User Manual (1)<BR>Updated: 2018-03-24<BR><A HREF="#index">Index</A>
<A HREF="/cgi-bin/man/man2html">Return to Main Contents</A><HR>

<A NAME="lbAB">&nbsp;</A>
<H2>NAME</H2>

qdda - the quick &amp; dirty dedupe analyzer
<A NAME="lbAC">&nbsp;</A>
<H2>SYNOPSIS</H2>

<B>qdda &lt;options&gt; [FILE...]</B>
<P>
<A NAME="lbAD">&nbsp;</A>
<H2>DESCRIPTION</H2>

<B>qdda</B>
checks files, data streams or block devices for duplicate blocks to estimate deduplication
efficiency on dedupe capable storage systems, using key-value stores in SQLite,
MD5 hashing and LZ4 compression.  It also estimates compression ratios for all-flash arrays
XtremIO X1 and X2 as well as VMAX AFA (experimental).
<P>

<P>
<A NAME="lbAE">&nbsp;</A>
<H2>IMPORTANT NOTES</H2>

<B>qdda</B>
can create very large database files and generate lots of read I/O and heavy CPU load. Check the 
<B>RESOURCE REQUIREMENTS</B>
section before you start.
