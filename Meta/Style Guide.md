---
tags: miscellaneous todo
---
# Style Guide
This page details the style guide for this wiki.
^summary

## Structure
### In-universe content
All in-universe content goes in the `Wiki` folder, organised into the following types:

- Characters
- Concepts
- Creatures
- Events
- Groups
- Locations
- Miscellaneous
- Objects

Each page must belong to one of these types, and is also [[#Metadata|tagged]] as such.

### Other content
The following other content also exists on this wiki:

#### Campaigns
Goes in the `Meta/Campaigns` folder.

#### DM Notes
The `_DM Notes` folder is used for larger, completely private notes. It doesn't need to use any of this guidance, unless snippets in there are being written as a "staging area" of sorts to be included in the main wiki later. This separation is useful for potentially making the wiki available to players in the future.

#### Sessions
Goes in the `Meta/Sessions/[Campaign Name]` folder. One-shots stay in the `Meta/Sessions` folder.

## Writing style
For the most part, the writing style should **mimic other major wikis**. Wikipedia, Wookieepedia, and the TARDIS Wiki are three major examples.

All in-universe content should be written in the **past tense**, regardless of how relevant it is to currently running campaigns --- imagine this wiki is a little like a history book in that respect. This is so we don't have to go back and revise pages later on when they aren't current.

## Page formatting
### Layout
All articles adhere to this rough layout:

1. YAML metadata, title
2. Opening summary *(marked with `^summary` tag)*
3. Main article *(varies by page type)*:
	1. Further major details *(e.g. "Properties" for Objects type)*
	2. History
	3. Further lesser details *(e.g. "Personality" for Creatures type)*
	4. Links to relevant people/groups/locations etc.
4. Other Notes

### Templates
The page type templates in `_Templates` should be used for every new wiki page. They produce the layout above, pre-tailored to each type.

#### Snippets
Aside from the basic page type templates, various smaller snippets are also available:

- ***Title:*** Useful for non-wiki pages or DM Note pages. Avoid using for wiki pages.
- ***DM Note:*** For inline DM notes in wiki pages, that are hidden upon rendering. Useful for if/when I eventually make this wiki public.

### Headings
Page titles and headings should be written in "sentence case". For example, *"Fall of the human kingdoms"* is correct, whereas *"Fall of the Human Kingdoms"* is incorrect.

Avoid using articles such as *a/an/the* before page titles and headings. Using them in links is recommended however, to help extend the clickable area.

A h1 tag is used for the page title. Page contents should **only** use h2 to h4. The only exceptions to this are:

- ***Tables*:** May optionally use a h6 as a preceding caption
- ***DM Note snippets*:** Preceded by a h5, and may optionally use h6 for subheadings in complex cases --- this should be avoided where possible.

For further organisation below a h4, you can use either the D&D-style subparagraph (***bold-italics*** at the start of a paragraph), bulleted lists, or both. If this still causes unclear organisation in a page, it may be worth revisiting its overall structure or splitting certain sections off into their own pages.

### Content
#### Summary
Each page **must** have an opening summary (marked with the `^summary` tag for easy embedding). The title/focus of the the page should also be bolded in the summary as well, alongside any alternate names. Translations should be quoted in italics instead of bold.

###### Examples
> The **Khal'syrat** (*"divine tools"* in Celestial) was a trinity of objects...

> **Astral amber** (often simply referred to as **amber**) was a hardened substance...

#### Paragraphs
Paragraphs should start on the line directly below a heading, with blank lines separating them afterwards. There should also be a blank line before each heading (aside from the page title).

#### Quotes and lists
Quotes and lists should be surrounded by a blank line before and after them. The blank line before is skipped if the item is directly below a heading.

Avoid going further than 3 levels deep in a list --- ideally 2 is the limit. If you find yourself needing to make deeper lists, consider if the top level should be subheadings instead.

#### Non-ASCII characters
- Avoid "smart" (curly) quotation marks and apostrophes, and use the ASCII ones (`'` and `"`).
- Latin extended characters such as accents are allowed as part of names, fictional language words etc.
- Dashes should use `---` for a long dash (for breaking up sentences), or `--` for a short dash (number ranges). Long dashes should have a space on either side, because I'm weird.

## Metadata
Currently the ability to use metadata in Obsidian is limited.

### Tags
The main metadata used across all pages (aside from DM notes) is **tags**. Tags are placed as the last item in the metadata, are lowercase and hyphenated, and added in the following order:

1. Page type
2. Other subcategories
3. Relevant campaigns:
	- These can be found in each campaign page, e.g. [[Meta/Campaigns/Blackbird]] uses #blackbird
	- One-shots get their own tag, as well as the #one-shots tag
4. Further modifiers:
	- #todo for incomplete pages
	- #from-sourcebooks for items that are pulled directly from the *Scum & Villainy* books

For pages that have "children", the campaign tags should only be on the pages that were directly relevant to the campaign, to help minimise clutter in search results (as these parent pages are almost always linked in the children anyway). For example, [[Seraph]] and [[Triumph Station]] have the #blackbird tag, but its parent location (the [[Boros System]]) doesn't have that tag unless the characters explicitly visit another location there.

### Campaign metadata
Campaigns have the following YAML metadata:

```yaml
start_date: 2022-01-01
end_date: Ongoing
```

- `start_date` *(mandatory)* must be an [ISO 8601 date](https://www.iso.org/iso-8601-date-and-time-format.html) - the timestamp isn't needed.
- `end_date` *(mandatory)* must either be:
	- An ISO 8601 date
	- One of these strings: *"Ongoing"*, *"On Hiatus"*, or *"Cancelled"*.

### Character metadata
Characters have the following YAML metadata:

```yaml
player: Louis
status: Active
```

- `player` *(mandatory)* is the name or nickname of the player.
- `status` *(mandatory)* must either be:
	- *"Active"*
	- *"Away"* --- player is on extended hiatus (i.e. more than a session or two)
	- *"Missing"* --- character's fate unknown and/or player permanently unavailable
	- *"Retired"* --- character's fate known (still alive, but unable to return)
	- *"Deceased"*

### Session metadata
Sessions have the following YAML metadata:

```yaml
date: 2022-01-01
```

- `date` *(mandatory)* must be an ISO 8601 date.

## Useful Links
- https://en.wikipedia.org/wiki/Wikipedia:Manual_of_Style
- https://starwars.fandom.com/wiki/Wookieepedia:Manual_of_Style
- https://tardis.fandom.com/wiki/Category:Manual_of_style
