## Blog
[![CircleCI](https://circleci.com/gh/emoji-gen/blog/tree/master.svg?style=shield)](https://circleci.com/gh/emoji-gen/blog/tree/master)
[![Requirements Status](https://requires.io/github/emoji-gen/blog/requirements.svg?branch=master)](https://requires.io/github/emoji-gen/blog/requirements/?branch=master)
[![dependencies Status](https://david-dm.org/emoji-gen/blog/status.svg?path=theme)](https://david-dm.org/emoji-gen/blog?path=theme)
[![devDependencies Status](https://david-dm.org/emoji-gen/blog/dev-status.svg?path=theme)](https://david-dm.org/emoji-gen/blog?path=theme&type=dev)
[![devDependencies Status](https://david-dm.org/emoji-gen/blog/dev-status.svg)](https://david-dm.org/emoji-gen/blog?type=dev)

## Requirements

- Python `$(cat .python-version)`
- Node `$(cat .node-version)`
- Yarn

## Libraries

- [Pelican](https://github.com/getpelican/pelican)
- [Normalize.css](https://necolas.github.io/normalize.css/)

## Getting started

```bash
# Setup Python
$ python -m venv venv
$ . venv/bin/activate
$ pip install -r requirements-dev.txt

# Setup Node
$ yarn
$ cd theme && yarn

# Development
$ make dev
```

## Development
### Pygments

```bash
$ pygmentize -S trac -f html -a .highlight > theme/src/generated/pygments.css
```

## Deployment

```bash
$ yarn global add firebase-tools

$ make            # Build for production
$ firebase deploy # Deployment
```

## License
MIT &copy; [Emoji Generator](https://emoji-gen.ninja/)
