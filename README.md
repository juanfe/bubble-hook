# bubble-hook
Code sniffer to prevent debug lines in ruby, python, and js.

Author: Juan Fernando Jaramillo Botero <juanf.jaramillo@opdevel.com>
Website: http://github.com/juanfe/bubble-hooks

REQUIREMENTS

 * Bash

FEATURES

 * Check by the occurrence of: "binding.pry" in *.rb, or *.erb
 * Check by the occurrence of: "console.log" in *.js, or *.coffee
 * Check by the occurrence of: "import pdb" in *.py


USAGE

 * Put the script "pre-commit" into your .git/hooks directory 
 * OR: add the script to your pre-commit "chain" (you probably know what to do then)
 * Put the Config file "config" into the same dir as the "pre-commit" script and
   edit it to your requirements
 * Ensure that the script is executable, by using:
     > chmod +x .git/hooks/pre-commit
