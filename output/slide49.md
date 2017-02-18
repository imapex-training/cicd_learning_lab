
### Steps
1. Open the _.drone.yml_ file in your editor.  The file should begin looking like the code block below.  The _build_ directive at the top represents where the integration phase of the process will take place.  

In the _commands:_ list under _run_tests:_ are the different steps needed to test a successful code change.

```
build:
  build_starting:
    image: python:2
    commands:
      - echo "Beginning new build"	
```

