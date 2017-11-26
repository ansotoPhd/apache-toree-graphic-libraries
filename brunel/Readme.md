Brunell <--> One jar library with a toree magic

- Option 1: loading inside a notebook

'''
%AddJar -magic https://brunelvis.org/jar/spark-kernel-brunel-all-2.5.jar
'''

- Option 2: loading when the Apache toree kernel starts

kernel.json file:

  "argv": [
    ...
    "--profile", "{connection_file}",
    "--magic-url", "file:/home/astwin/workspace/spark-kernel-brunel-all-2.5.jar"	
    ...



=> Problems:

https://github.com/Brunel-Visualization/Brunel/issues/243

https://issues.apache.org/jira/browse/TOREE-439
