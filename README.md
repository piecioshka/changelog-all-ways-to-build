# changelog - ways to create this file

How to build a changelog?

> Article in Polish: https://piecioshka.pl/blog/2019/03/23/husky-commitlint-git-changelog.html

## tool: git-changelog

```bash
npx git-changelog -e
npx git-changelog -t false -a 'Angular: Spy LifecycleHooks'
```

## tool: generate-changelog

```bash
npx generate-changelog -M # major
npx generate-changelog -m # minor
npx generate-changelog -p # patch
```

feedback:

- beznadziejne, nie wiadomo jak tego używać

## tool: changelog

```bash
npx changelog piecioshka/dotfiles all
```

feedback:

- MINUS: nie zapisuje do pliku

## tool: auto-changelog

```bash
npx auto-changelog -u -l false
```

template:

- https://github.com/piecioshka/super-event-emitter/blob/d68ab7d88fc94e3f8894232dd427bf5a07d86910/.github/CHANGELOG_TEMPLATE.hbs#L4
- .github/CHANGELOG_TEMPLATE.hbs

examples:

- https://github.com/piecioshka/super-event-emitter

## tool: git-extras

Use https://github.com/tj/git-extras/blob/master/Commands.md#git-changelog:

```bash
git changelog -a -n -p
```

examples:

- https://github.com/piecioshka/boilerplate-jasmine-babel?tab=readme-ov-file

## tool: conventional-changelog

```bash
npx conventional-changelog -i CHANGELOG.md -s -r 0
# Angular
npx conventional-changelog -p angular -i CHANGELOG.md -s -r 0
```

## tool

```bash
npx @angular/cli changelog
```
