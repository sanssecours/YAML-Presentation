# “Minimally” Useful 🐪 YAML Features for Elektra

## 📋 Lists

- [ ] Flow Style (`[value 1, value 2]`)
- [ ] Block Style

    ```yaml
    - value 1
    - value 2
    ```

## 🗺 Mappings

- [ ] Flow Style (`{key: value, another key: another value}`)
- [ ] Block Style

    ```yaml
    key: value
    another key: another value
    ```

- [ ] Support for Complex Keys

    ```yaml
    ?
    - { 'pretty': complex key }
    - - 😱
    - Still part of the key
    : value
    ```

## 📏 Scalars

- Flow Scalars
  - [ ] Plain (`Some Data`)
  - [ ] Single Quoted (`'Single Quotes'`)
  - [ ] Double Quoted (`"First Line\nSecond Line"`)
- Block Scalars
  - [ ] Folded

    ```yaml
    > # "One Two"
      One
      Two
    ```

  - [ ] Literal

    ```yaml
    | # "One\nTwo"
      One
      Two
    ```

  - [ ] Indentation Header (`>1`, `|4`)
  - [ ] Chomping Header (`|- `, `>+`)

## 🗃 Multiple Documents

- [ ] Support Streams

## 🐠🐙🐶 Types

### 📢 Directives

- [ ] YAML Version (`%YAML 1.2`)
- [ ] TAG Handle Definition (`%TAG !! tag:yaml.org,2002:`)
  - [ ] Named Tag Handle (`!name!suffix`)

###  🏷 Tags

#### Tag Shorthands

- [ ] Primary Tag Handle (Default Resolution: `!`) (`!suffix`)
- [ ] Secondary Tag Handle (Default Resolution: `tag:yaml.org,2002:` ) (`!!suffix`)

#### Verbatim Tags

- [ ] Local Tag (`!<!local>`)
- [ ] Global Tag (`!<global>`)

#### Other Tags

- [ ] Non-Specific Tag (`!`)

### 📚 Schemas

- [ ] Failsafe Schema (`!!str`, `!!seq`, `!!map` )
- [ ] JSON Schema (Failsafe Schema  + `!!null`, `!!bool`, `!!int`, `float`)
- [ ] Core Schema (JSON Schema + `0x9abc`, `0o678`, `~`, …)
- [ ] Additional Types (`!!omap`, `!!set`, `!!binary`, `!!timestamp`, …)
  - Which Ones:

## ⚓️ References

- [ ] Support Anchors & Aliases
