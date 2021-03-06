Copyright �2014 . John Scancella (Regents). All Rights Reserved. Permission to use, copy, modify, and distribute this software and its documentation for educational, research, and not-for-profit purposes, without fee and without a signed licensing agreement, is hereby granted, provided that the above copyright notice, this paragraph and the following two paragraphs appear in all copies, modifications, and distributions. Contact John Scancella, for commercial licensing opportunities.

Created by John Scancella

IN NO EVENT SHALL REGENTS BE LIABLE TO ANY PARTY FOR DIRECT, INDIRECT, SPECIAL, INCIDENTAL, OR CONSEQUENTIAL DAMAGES, INCLUDING LOST PROFITS, ARISING OUT OF THE USE OF THIS SOFTWARE AND ITS DOCUMENTATION, EVEN IF REGENTS HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

REGENTS SPECIFICALLY DISCLAIMS ANY WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE. THE SOFTWARE AND ACCOMPANYING DOCUMENTATION, IF ANY, PROVIDED HEREUNDER IS PROVIDED "AS IS". REGENTS HAS NO OBLIGATION TO PROVIDE MAINTENANCE, SUPPORT, UPDATES, ENHANCEMENTS, OR MODIFICATIONS.


Route-able deliverance
====================================================
requirements:
 1) must be able to search multiple directories for files
 2) must be able to route files through multiple servers 
 2) must have an easy to use GUI
	a) text area to add servername or ip address
	b) regex listing for file types
	c) drag and drop connecting regex to ip address
	d) browsable menu for which directories to search
 3) must be able to be configurable through GUI, command-line, and xml/properties
 4) if a server is unavailable to receive the file being routed then:
	a) if possible routes it to another server or:
	b) waits until the server is available to send the file
 5) must be able to configure each server hop with a different username/password/account if wanted
 6) Nice to have, automatic server discovery

 



COMMANDS:
=====================================================

to update eclipse run
===================================
gradle cleanEclipse eclipse

to build and run application run
===================================
gradle clean bootRepackage && java -jar build/libs/Hermes.jar

debug
===================================
java -Xdebug -Xrunjdwp:transport=dt_socket,address=1000,server=y,suspend=n -jar build/libs/Hermes.jar