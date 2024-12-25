# Binary execution speed improvement

My solution is improve the performance or reduce startup execution time as for `pre-commit`, `pre-push` or on something or even at calling on CI/CD it could work faster thus reducing cost of CI/CD or reduce energy usage on local thus saving the battery. Helping to both CPU and nature to reduce carbon by saving power is good reason to try it.

## Attempt 1

> [!CAUTION]
> Status: Failed or Rejected

Date: April 07 - April 09 at 2024

### Title: Find `platform` `bin` and replace link to that `bin`

### Alt title: Direct bin call

### Issues or Discussions

| Project  | Issue or Discussion                                    |
| -------- | ------------------------------------------------------ |
| dprint   | https://github.com/dprint/dprint-plugin-json/issues/35 |
| biomejs  | https://github.com/biomejs/biome/discussions/2315      |
| jsona    | https://github.com/jsona/jsona/issues/52               |
| lefthook | https://github.com/jsona/jsona/issues/52               |

### Solutions provided

| Project | PR                                           |
| ------- | -------------------------------------------- |
| dprint  | https://github.com/dprint/dprint/pull/839    |
| dprint  | https://github.com/dprint/dprint/pull/840    |
| biomejs | https://github.com/biomejs/biome/pull/2359   |
| oxc     | https://github.com/oxc-project/oxc/pull/2920 |

### Excepted

Like this solution: https://github.com/evanw/esbuild/blob/main/lib/npm/node-install.ts

## Attempt 2

> [!CAUTION]
> Status: Failed or Rejected

Date: April 12 - April 15 at 2024

### Title: Using `platform` packages `bin` and require by `engines`

### Alt title: Link `platform` `bin` to project main `package`

### Issues or Discussions

| Project  | Issue or Discussion                                 |
| -------- | --------------------------------------------------- |
| lefthook | https://github.com/evilmartians/lefthook/issues/703 |

### Solutions provided

| Project  | PR                                                |
| -------- | ------------------------------------------------- |
| lefthook | https://github.com/evilmartians/lefthook/pull/705 |

## Attempt 3

> [!CAUTION]
> Status: Failed or Rejected

Date: July 30 - August 01 at 2024

### Title: shell `bin.sh` solution to execute

### Issues or Discussions

| Project  | Issue or Discussion                               |
| -------- | ------------------------------------------------- |
| biomejs  | https://github.com/biomejs/biome/discussions/2315 |
| lefthook | https://github.com/jsona/jsona/issues/52          |

### Solutions provided

| Project  | PR                                                |
| -------- | ------------------------------------------------- |
| biomejs  | https://github.com/biomejs/biome/pull/3550        |
| lefthook | https://github.com/evilmartians/lefthook/pull/798 |
