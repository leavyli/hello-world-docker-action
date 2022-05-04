## notice
on windows,  when you use chmod command +x  for entrypoint.sh in git bash，  then you still should overwriter execute bit as fllow git commands. 
(https://github.community/t/permission-denied-exec-entrypoint-sh/16216)

``` shell
git add --chmod=+x -- entrypoint.sh
git commit

```

# Hello world docker action

This action prints "Hello World" or "Hello" + the name of a person to greet to the log.

## Inputs

## `who-to-greet`

**Required** The name of the person to greet. Default `"World"`.



## Outputs

## `time`

The time we greeted you.

## Example usage

uses: actions/hello-world-docker-action@v1
with:
  who-to-greet: 'Mona the Octocat'
  
