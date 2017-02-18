
2. Since we are **NOT** changing the actual build process stored in `.drone.yml`, we don't need to recreate the secrets file.  Once the build process is complete, as long as new tests or steps aren't added these files can be left alone.  Developers can focus on their code and changes, not the build process.

