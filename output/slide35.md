
### Steps
1. The drone utilities on your laptop need to know the address and access information for the drone server you are using.  We use session environment variables for this. You will replace the variable's value with the information the lab admin gives you. The follow code can be copied and pasted directly into a terminal window if you'd like to do that, but you can also just type in the line that doesn't start with the hash mark.

    ```
    # Configure the drone server address,
    # Use the address provided by the lab administrator
    export DRONE_SERVER=http://DRONE_SERVER
    ```

