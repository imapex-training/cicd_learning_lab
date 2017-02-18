
2. Now we will add Testing to the *build* phase.  Update `.drone.yml` to match the updated content below. In the _commands:_ list under _run\_tests:_ are the different steps needed to test a successful code change.  
	* **NOTE You can simply copy and paste the contents from below directly into your file.**

```
build:
    build_starting:
        image: python:2
        commands:
            - echo "Beginning new build"
    run_tests:
        image: python:2-alpine
        commands:
            - pip install -r requirements.txt
            - python testing.py
```

