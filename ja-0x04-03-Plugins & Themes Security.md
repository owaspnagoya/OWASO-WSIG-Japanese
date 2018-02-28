
== Plugins & Themes Security ==
Plugins and themes are a great addition to the functionality offered by the WordPress core. WordPress’ success is based on these elements. It’s easy to develop a new theme, add new functions with plugins. This ease of development comes with the security downside. In the rush for functionality, the developers often forget about security. Looking at the [https://cve.mitre.org/cgi-bin/cvekey.cgi?keyword=wordpress CVE list for WordPress] it’s worth noticing that in the past years most of the security defects are affecting the plugins and themes and not WordPress core.

Developing on top of WordPress should be regarded as a regular development job and follow a standard secure development lifecycle. Concrete action items for this chapter include source code review and penetration testing of plugins and themes.

When choosing to use an already developed plugin by a 3<sup>rd</sup> party, a security audit should be performed. Good differentiators for available plugins are:

* Publication in the official plugin store at https://wordpress.org/plugins/
* User ratings and comments
* Version number (is it a young plugin/theme or has it faced the challenges of time?)
* Last update 
* Update frequency 
* Compatibility with the current version of the WordPress core

In order to perform a source code audit, the following tools can be used:

* [http://rips-scanner.sourceforge.net/ RIPS]
* [http://www.program-transformation.org/PHP/PhpSat PHP-sat]
* [http://www.scovetta.com/yasca.html Yasca]
* [http://resources.infosecinstitute.com/finding-bugs-in-php-using-grep/ Manual analysis using grep], [https://grepbugs.com/ GrepBugs]

Things to pay extra attention during the source code audit:

* Obfuscated code
* BASE64 encode function
* System call functions (exec, passthru, system, shell_exec, etc.)
* PHP code execution (eval, assert, preg_replace, etc.)
* Information disclosure functions (phpinfo, getenv, getmygid/pid/uid, etc.)
* Filesystem functions (fopen, bz/gzopen, chgrp/own/mod, etc.)

