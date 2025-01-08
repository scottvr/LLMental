# [LLMental:](https://github.com/scottvr/LLMental) 
LLMental - pronounced like "elemental" ˌe-lə-ˈmen-tᵊl *adj*
- of, relating to, or being the basic or essential constituent of something : FUNDAMENTAL
- A collection of tools to make pair-programming with LLMs more productive and less context/memory/token/dollar expensive.

## This meta-repo contains the following github repos as git submodules:

- ### [phart:](https://github.com/scottvr/phart)
The Python Hierarchical ASCII Representation Tool - A Pure Python graph visualization in ASCII. Built for networkx, but also supports DOT and graphml inputs. Python API w/cli. Stable releases at PyPi (installable via `pip install phart`

- ### [retree:](https://github.com/scottvr/retree)
Python tool that essentially inverts what /usr/bin/tree -F does. It creates a real directory structure on your filesystem based on an ascii line-art tree (or the output of ls -lR or find. etc). READMEs and LLMs often suggest directory structures via a tree or tree-like fenced ascii-block. This tool automates creating the files and dirs in that tree. (Also implemented in typescripts as a vscode extension so you can highlight such a tree within your IDE and have the tool do the needful. ALso, a bonus implementation in 100% bash (to answer a question on SO and for the lulz.)

- ### [ſplit:](https://github.com/scottvr/fplit)
fplit (file + split, as it might look in the 1700's (long/medial "s" can look to us like a lower-case 'f') takes Python scripts containing multiple function demonstrations (typically in a __main__ block or at module level) and splits them into separate, self-contained files. It intelligently preserves necessary context like imports, setup code, and related statements. This one began to grow out of hand with each larger list of "most popular python modules" I'd find and add support for.

- ### [maxify:](https://github.com/scottvr/maxify)
Maxify is a command-line tool that automates the unpacking and deminification of JavaScript projects from sourcemap files (with sourcesContent keys).  This one wasn't developed as part of the goal of beefing up the pairing-with-LLM process, but since it is a tool that I wrote for a one-off need, then added cli arguments, etc, I'm listing it here.

- ### [crumb.py:](https://github.com/scottvr/crumb.py)
Simply (but carefully and configurably) tags near the top of a .py file the relative path name of the file at the time of tagging.  This should hopefully not be relevant for all that much longer in the context fo sharing files with LLMs, but presently both ChatGPT and Claude have a concept of "Projects" to which you can upload files to remain in context for any chats started under the project, but they are limited to flate namespace for files. This is a way to put a comment in the files before uploading that informs the reader what its relative path should be understood to be.

- ### [ccat:](https://github.com/scottvr/chimeracat)
ccat - ChimeraCat smart code concatenator. Originally just concat'd .py files so you could paste them into an .ipynb notebook without having to upload a bunch of files and deal with import paths etc in an environment such as colab, it grew with a dependency graph and ability to output an ipynb notebook directly. Further it analyses files to determine the best order to concatenate them in, and to eliminated duplicates and perpetual recursive import loops. In addition it can strip boilerplate code and make other intelligent choices about what to leave out, and the heuristics are fully user defineable via custom configuration rules (also written in python.)
