# changelog - all ways to build

How to build a changelog?

> My article in Polish 🇵🇱: https://piecioshka.pl/blog/2019/03/23/husky-commitlint-git-changelog.html

## tool: [git-changelog](https://npmjs.com/package/git-changelog) [[source code](https://github.com/rafinskipg/git-changelog)]

```bash
npx git-changelog -e
npx git-changelog -t false -a 'Angular: Spy LifecycleHooks'
```

## tool: [generate-changelog](https://www.npmjs.com/package/generate-changelog) [[source code](https://github.com/lob/generate-changelog)]

```bash
npx generate-changelog -M # major
npx generate-changelog -m # minor
npx generate-changelog -p # patch
```

feedback:

- MINUS: hard to use it, it's not intuitive tool

## tool: [changelog](https://www.npmjs.com/package/changelog) [[source code](https://github.com/dylang/changelog)]

```bash
npx changelog piecioshka/dotfiles all
```

feedback:

- MINUS: do not save into file

## tool: [auto-changelog](https://www.npmjs.com/package/auto-changelog)[[source code](https://github.com/CookPete/auto-changelog)]

```bash
npx auto-changelog -u -l false
```

feedback

- PLUS: use template

templates examples (`.github/CHANGELOG_TEMPLATE.hbs`):

- [super-event-emitter](https://github.com/piecioshka/super-event-emitter/blob/d68ab7d88fc94e3f8894232dd427bf5a07d86910/.github/CHANGELOG_TEMPLATE.hbs#L4)

project examples:

- [super-event-emitter](https://github.com/piecioshka/super-event-emitter/blob/master/CHANGELOG.md)

## tool: [git-extras](https://github.com/tj/git-extras/blob/master/Commands.md#git-changelog) [[source code](https://github.com/tj/git-extras)]

```bash
git changelog -a -n -p
```

project examples:

- [boilerplate-jasmine-babel](https://github.com/piecioshka/boilerplate-jasmine-babel/blob/master/CHANGELOG.md)

## tool: [conventional-changelog](https://www.npmjs.com/package/conventional-changelog-cli) [[source code](https://github.com/conventional-changelog/conventional-changelog)]

```bash
npx conventional-changelog -i CHANGELOG.md -s -r 0
# for Angular projects with convention eg. "chore(...)"
npx conventional-changelog -p angular -i CHANGELOG.md -s -r 0
```

## tool: [@angular/cli](https://www.npmjs.com/package/@angular/cli) [[source code](https://github.com/angular/angular-cli)]

```bash
npx @angular/cli changelog
```
