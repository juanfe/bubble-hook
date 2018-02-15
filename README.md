# bubble-hook

Codesniffer to prevent undesired debug bubble in code of Ruby, Python or JS.

Author: Juan Fernando Jaramillo Botero <juanf.jaramillo@opdevel.com>
Website: http://github.com/juanfe/bubble-hooks

## REQUIREMENTS

 * Bash

## FEATURES

 * Check occurrence of 'binding.py' in files withe extension "*.rb" or "*.erb".
 * Check occurrence of 'console.log' in files withe extension "*.js" or "*.coffee".
 * Check occurrence of 'import pdb' or 'import ipdb' in files withe extension "*.py".


## USAGE

 * Put the script "pre-commit" into your .git/hooks directory 
 * OR: add the script to your pre-commit "chain" (you probably know what to do then)
 * Put the Config file "config" into the same dir as the "pre-commit" script and edit it to your requirements
 * Ensure that the script is executable. 
 * You can turn off the sniffer by:
   > git config hooks.allowbubble true
 * You can turn on the sniffer again by:
   > git config hooks.allowbubble false

## REFERENCE:
 [1] http://codeinthehole.com/writing/tips-for-using-a-git-pre-commit-hook/
 [2] https://github.com/s0enke/git-hooks
 [3] .git/hooks/pre-commit.sample
