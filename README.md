# php-list-api

## Motivation

I wanted to have a clone of the GitHub API, in PHP (it can be used on simple host server which use PHP)

## Variable to change

- the link in `.htaccess`
- the path in `$GLOBALS['path']`

## Testing

Run a simple command

```sh
bash build.sh
```

Then go to `localhost:8080`


## Examples

### `http://localhost:8080/expose/`

```json
[
    {
        "name": "file.txt",
        "path": "file.txt",
        "sha": "e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855",
        "size": 0,
        "url": "",
        "html_url": "-",
        "git_url": "-",
        "download_url": "-",
        "type": "file"
    },
    {
        "name": "folder",
        "path": "folder/",
        "sha": "0",
        "size": 0,
        "url": "",
        "html_url": "-",
        "git_url": "-",
        "download_url": "-",
        "type": "dir"
    }
]
```

### `http://localhost:8080/expose/file`

```json
{
    "message": "Not Found",
    "documentation_url": "no"
}
```
