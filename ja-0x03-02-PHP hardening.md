# PHP hardening
* 常に最新にする


* Update regularly
* Don’t install PHP as a CGI binary
* Disable unnecessary PHP modules
* Disable unused potentially dangerous PHP functions (good examples: ''exec'',''passthru'',''shell_exec'',''system'', etc.)
* Log errors internally
* Disable verbose error reporting on the client side
* Turn off remote code execution (if it’s not needed; the core WordPress doesn’t need this functionality)
* Disable magic quotes
* Limit PHP access to file system
* Protect from DoS
** Control POST size
** Limit script time execution
** Limit memory usage
* Consider implementing the [http://www.suhosin.org/stories/index.html Suhoshin security extension]
* Hide the version of PHP in use
* Hide the .php extension
