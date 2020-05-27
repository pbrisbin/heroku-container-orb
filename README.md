# Heroku Container Orb [![CircleCI status](https://circleci.com/gh/pbrisbin/heroku-container-orb.svg "CircleCI status")](https://circleci.com/gh/pbrisbin/heroku-container-orb)

Build, push, and release using `heroku:container` commands.

See https://devcenter.heroku.com/articles/container-registry-and-runtime.

## Usage

```yaml
version: 2.1

orbs:
  heroku-container: pbrisbin/heroku-container@x.y

workflows:
  push_and_release:
    jobs:
      - heroku-container/push-and-release:
          app-name: some-app-name
```

See [all examples](./src/examples/).

---

[LICENSE](./LICENSE) | [CHANGELOG](./CHANGELOG.md)
