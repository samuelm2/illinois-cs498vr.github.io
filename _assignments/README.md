
## Managing Assignments

Assignments are defined in the `_assignments/` folder. The frontmatter YAML schema is as follows:

- `layout: mp`
- `title`: string, used as the header
- Either: `due` or `parts`:
	- `due`: string, literal due date for single-part MP
	- `parts`: list of objects
		- `title`: string, name of part (e.g. "MP1.1"), listed under due dates.
		- `due`: string, bolded and inserted next to part title.
- `material`: optional list of objects, containing:
	- `name`: string, name to display for this link.
	- `url`: string, URL to resource.
- `points`: string/number, total number of points an assignment is worth.
- `rubric`: list of objects
	- `name`: string, a short name for the item
	- `points`: number, the point value of this item
	- `description`: string, a longer text-only description of the item
- `notes`: optional boolean, default true, specifies whether to render `important_notes.md` above the `content`
- `instructions`: optional boolean, default true, specifies whether to render `submission_instructions.md` below the `content`
