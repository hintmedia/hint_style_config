# Hint Base Style and Linter Config

This repo contains our current base configs for style and linting.

## Rubocop Setup

In `.rubocop.yml` add the follow to get started using the hint rubocop config.

```yaml
inherit_from:
  - https://raw.githubusercontent.com/hintmedia/hint_style_config/master/.hint_rubocop.yml

AllCops:
  TargetRubyVersion: PROJECT_RUBY_VERSION
  TargetRailsVersion: PROJECT_RAILS_VERSION
  DisplayCopNames: true
  Include:
    - '**/Rakefile'
    - '**/config.ru'
  Exclude:
    - 'bin/**/*'
    - 'config/**/*'
    - 'db/**/*'
    - 'Gemfile*'
    - 'script/**/*'
    - 'test/**/*'
    - 'vendor/**/*'
```
Remove all other non-project specific settings.
