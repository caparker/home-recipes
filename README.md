# Meal Planning

## Weekly workflow
1. `cp templates/week.org weeks/$(date +%Y-W%V).org`
2. Open in Emacs, use gptel to draft menu from `meals.csv`
3. Fill in shopping list, commit, push
4. Copy shopping list into AnyList
5. Sunday next: fill in retro before starting new week

## Adding a recipe
1. `cp templates/recipe.md recipes/new-recipe-slug.md`
2. Fill in frontmatter + body
3. Add row to `meals.csv` (until recipes become source of truth)

## Conventions
- Slugs: kebab-case, match `meals.csv` names
- Week files: ISO week (`YYYY-Www`)
- Frontmatter: YAML, keep keys stable so we can script over them later
