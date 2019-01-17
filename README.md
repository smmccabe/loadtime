# Load Timer

Simple page load timer using firefox

## Usage

Provide a site to test.

```sh
$ loadtimer example.com
*** You are running in headless mode.
Time:		987 ms
Threshold:	5000 ms
Difference:	-4013 ms
```

Time includes starting Firefox headless and loading the page without caches.

If the test is not completed within the threshold the script exits with code 1. Otherwise it exits with code 0.

The threshold is 5 seconds by default. You can specify your own threshold in milliseconds.

```sh
$ loadtimer example.com 10000
*** You are running in headless mode.
Time:		987 ms
Threshold:	10000 ms
Difference:	-4013 ms
```
