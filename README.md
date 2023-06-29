# Parallax's Coding Style

## PHP (Laravel Pint)

### Installation

1\. Add the repository to your `composer.json` using either the JSON format:

```json
"repositories": {
    "parallax/coding-style": {
        "type": "vcs",
        "url": "https://github.com/parallax/coding-style.git"
    }
},
```

Or the CLI command:

```sh
composer config repositories.parallax/coding-style '{"type": "vcs", "url": "https://github.com/parallax/coding-style.git"}' --file composer.json
```

2\. Include `parallax/coding-style` in your project's dev dependencies:

```sh
composer require --dev parallax/coding-style
```

### Usage

Run the Pint command to apply the Parallax coding style:

```sh
./vendor/bin/pint --config vendor/parallax/coding-style/pint.json
```

You can also add a script to your `composer.json` for quicker style application:

```sh
composer config scripts.pint 'pint --config vendor/parallax/coding-style/pint.json' --file composer.json
```

Apply Parallax's coding style using the script:

```sh
composer pint
```
