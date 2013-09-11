# to_sentry
`to_sentry` is a really dumb command line sentry logger. 

# To use:

## Step #1: Install
```
pip to_sentry
```
## Step #2: Create `/etc/to_sentry.conf`

Use the read/write DSN sentry provided by each channel you want to log to.
```
[foo]
url=http://blabblabblab@sentryserver.example.com/13
 
[bar]
url=http://yadayadayada@sentryserver.example.com/42
```
## Step #3: Try it out
```
echo "hola mundo" | to_sentry foo "Hello World"  
```
