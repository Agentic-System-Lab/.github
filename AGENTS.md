# AGENTS.md

This repository is Agentic System Lab's public org profile. GitHub shows `profile/README.md` on
<https://github.com/Agentic-System-Lab> to everyone outside the org (members see the members-only profile first and can
switch to this one). The repository is public, so every file in it is public too, this one included.

## Public only

- Write nothing in any file here, commit messages included, that isn't public already. Name and link only public repos
  and public sites; a link to a private repo 404s for everyone outside the org. Tools that aren't public yet are
  described without their names (the "More tools are on the way" line). `gh repo list Agentic-System-Lab --json
  name,visibility` shows what is public.
- A push to `main` changes the org page at once. Preview first.

## The profile

- `profile/README.md` says what the homepage says: [agentic-system-lab.github.io](https://agentic-system-lab.github.io/)
  (`index.html` and `zh/index.html` in the homepage's repo, which is named after its domain). A change to a project's
  description, the study group or "How we work" goes into the profile and both pages. When a project goes public, add
  it to all three and take it out of the "on the way" sentence. That one sentence covers every tool not public yet, so
  remove it only when none is left.
- The profile is in English; it links to the Chinese homepage and to each project's Chinese README.
- It is GitHub-flavored Markdown, so styles and scripts are stripped. Images use absolute
  `https://raw.githubusercontent.com/Agentic-System-Lab/<public repo>/main/...` URLs, so they come from the project's
  own repo and stay current with it.
- Keep the voice of what is there: short, concrete sentences, with no superlatives. The intro speaks as "we"; a
  project's text tells the reader what they can watch and try.

Before pushing, check what GitHub makes of the Markdown (links, images, what it strips). This writes the rendered HTML
without GitHub's styles:

```sh
{ echo '<meta charset="utf-8">'; gh api -X POST /markdown -f mode=gfm -f context=Agentic-System-Lab/.github -f text="$(cat profile/README.md)"; } > /tmp/profile.html
```

## Files GitHub treats as org defaults

A community health file at this repository's root, in `.github/` or in `docs/` (`CODE_OF_CONDUCT.md`,
`CONTRIBUTING.md`, `SECURITY.md`, `SUPPORT.md`, `GOVERNANCE.md`, `FUNDING.yml`, issue and pull request templates,
discussion category forms) becomes the default for the org's repos that have none of their own, and
`workflow-templates/` offers its workflows to every repo in the org. Don't add any of these unless asked. AGENTS.md and
CLAUDE.md are not such files: they only guide work in this repository.

## Commits

English, with an imperative subject that says what changed; add a body on what and why when the subject doesn't make it
clear. Add a `Co-Authored-By:` line when an agent wrote the change.
