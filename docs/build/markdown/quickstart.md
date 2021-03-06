# Quickstart

Install packages

```
$ pip install pipenv
$ pipenv install
```

Create your configuration.yaml

```
configuration:
  environment: "<enviornment>"
  app_logging_level: "<logging-level>"
  global_logging_level: "<logging-level>"
environment:
  <environment>:
    sender:
      Discord:
        - name: "<bot-identifier>"
          token: "<discord-token>"
          activity:
            name: "<human-value>"
            type: "<discord-activity-type>"
          clean_channels:
            - <channel-id>
          reporting_channels:
            - <channel-id>
    receiver:
      Blackfire:
        colour: <integer-color>
        wait_time: <seconds>
        download_files: <true-or-false>
        search:
          "<string-to-search>":
            Discord:
              'Publisher':
                - <channel-id>
```

Run app

```
$ pipenv run
```
