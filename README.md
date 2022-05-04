# Hello world docker action

This action prints "Hello World" or "Hello" + the name of a person to greet to the log.

## Inputs

## `who-to-greet`

**Required** The name of the person to greet. Default `"World"`.

## notice
on windows, you should overwriter execute bit as fllow
(https://github.community/t/permission-denied-exec-entrypoint-sh/16216)

``` shell
git add --chmod=+x -- entrypoint.sh
git commit

```

## Outputs

## `time`

The time we greeted you.

## Example usage

uses: actions/hello-world-docker-action@v1
with:
  who-to-greet: 'Mona the Octocat'
  
