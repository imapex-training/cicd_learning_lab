
5. The build failed because we built the test **BEFORE** the feature.  That's test driven development, and the failure is exactly what we want to see.  When drone fails in the testing, the new container isn't built and published.  

