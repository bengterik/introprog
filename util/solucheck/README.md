# SOLUCHECK

This is a utility that checks the latex code in the compendum dir of this repo to see if the number of tasks and subtasks in exercises corresponds to the number of tasks and subtasks in solutions.

## Compile

    sbt compile
    
or

    scalac solucheck.scala

## Run


### Overview of diffs

To get an overview of all diffs:

    sbt "run --all"

or
    
    scala solucheck --all

### Diff report per week

To get a detailed report of the diffs of a specific week's exercises, e.g. week 02:

    sbt "run w02"

or 
    scala solucheck w02
    
    
ger nu dummy \Task och \Subtask för lika många som finns i övningen


### Init week

Before the first time you are making solutions for exercises in week XX:

    sbt "run --init wXX"

or

    solucheck --init wXX

This only works if there is no existing solution file so mv the existing solution file somewhere safe.

## Inspect the code and send bug reports as issues

Check out the code here:

https://github.com/lunduniversity/introprog/blob/master/util/solucheck/solucheck.scala

