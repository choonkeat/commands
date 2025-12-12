look at our git commits on top of origin/main and plan our pull request(s) to help reduce the burden for our reviewers

we'll create a code_reviews/{yyyy-mm-dd-HHMM in local time} to host our files:

	first, determine the commit(s) that will go into each pull request, e.g. startSHA to endSHA

	for each planned pull request write an .md file
	1. provide an overall title, in the style of conventionalcommit summary line
	2. provide an overall description (can be brief especially when we have good inline comments; see below)
	3. provide the commits
	4. provide inline comments pointing out salient or gist of the changes:
		- file content referenced must be as-of endSHA, i.e. git show endSHA:path/to/file
			- locate the code, as-of endSHA, that we want to point out in this pull request
			- cite the {filename}:{line number range} as-of endSHA
			- cite the code and add succinct comment right below the code
			- comment can highlight caveats, special note, interesting quirk, or significance to overall pull request
	5. for inline comments and overall description, when it makes sense to have a screen capture or screencast video, use mcp playwright (if mcp playwright is not setup, let me know how to do so before you proceed) to grab screenshot(s) and place png(s) alongside the markdown e.g. useful when code changes UI
	6. for any diagramming needs, prefer using ```mermaid code block

if any screenshots are better with before-and-after comparison, use a markdown table for side-by-side layout. tell me and i'll get the server running in base branch for you to grab all the "before" screenshots in one go.

$ARGUMENTS
