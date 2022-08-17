<p align="center">
  <img height="250" src="./logo.png" />
</p>

<h1 align="center"> JS-Barrels </h1>
<p align="center">
  <b>A CLI tool to generate barrels with ease, efficiency, and intelligence</b>
</p>

## Usage

```bash
npx js-barrels -d ./folder/to/generate/barrels/for
```

## Options

```bash
-d, --dir      Directory to generate barrels for           [string] [required]
-w, --watch    Watch and make barrels recursively                    [boolean]
-e, --ext      An extension to create the barrel file with, if not provided
               the script will determine based on the files in the dir[string]
```

## Motivation

After developing a Next.js project with many folders and files, I wanted to create barrels to easily use them without clutter in other files and directories, essentially trying to group imports cleanly with the barrels. After trying many different CLI solutions, I concluded that many of them did not fit my use case of default exports combined with named exports, so I set out to make my own CLI which supported both, hence the creation of this tool.

## Pros and Cons

### Pros

- Generates barrels for all exports including default and named
- Simplistic nature with only two CLI arguments
- Includes a watch mode to detect file changes and regenerate barrels accordingly
- Lightweight
- Generates barrels for nested directories
